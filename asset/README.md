# Testfeld Niedersachsen ALKS 3DModel opt osgb sample

Motorway section of the test field Lower Saxony with 2000x2000m size with 1x1 tiles.

## Digital Assets

This is a digital asset according to the ENVITED Ecosystem Specification [EVES-003](https://ascs-ev.github.io/EVES/EVES-003/eves-003.html) for the ENVITED-X Data Space. It can be used as a template for other dataspaces as well. It contains a fully described and consistent example of a digital asset including a **`manifest_referene.json` - file** as content registry.

A complete **`digital asset`** in a specific domain includes the data itself and all necessary files for describing, evaluating, and visualizing the dataset.

## Example Asset Folder Structure

This sample **`digital asset`** can be downloaded from the [GAIA-X4PLC-AAD/environment-model-asset-example](https://github.com/GAIA-X4PLC-AAD/environment-model-asset-example) as artifact of the lastest release (**`asset.zip`**) containing the following structure:

📁 `asset`

- 📁 `simulation-data`
  - 📄 `Gaia_X_Example_Asset_TestfeldNiedersachsen_ALKS_3DModel_opt_osgb.zip`
- 📁 `documentation`
  - 📄 `Gaia_X_Example_Asset_TestfeldNiedersachsen_ALKS_3DModel_opt_osgb_TRIANxUNITY_Full_Workflow_Documentation.pdf`
  - 📄 *`assetName_[Name].[ext]`* <i style="color:gray;">(optional)</i>
- 📁 `metadata`
  - 📄 `environment-model_instance.json`
- 📁 *`validation-reports`* <i style="color:gray;">(optional)</i>
  - 📄 *`qcReport.txt`* <i style="color:gray;">(optional)</i>
- 📁 `media`
  - 📄 `Gaia_X_Example_Asset_TestfeldNiedersachsen_ALKS_3DModel_opt_osgb_impression-01.png` *-> eyecatcher*
  - 📄 *`Gaia_X_Example_Asset_TestfeldNiedersachsen_ALKS_3DModel_opt_osgb_impression-02.png`* *-> impression* <i style="color:gray;">(optional)</i>
  - 📄 *`Gaia_X_Example_Asset_TestfeldNiedersachsen_ALKS_3DModel_opt_osgb_impression-03.png`* <i style="color:gray;">(optional)</i>
- 📄 `README.md`
- 📄 `manifest_reference.json`

### Legend

- 📁 `folder-name`: A folder in the repo.
- 📄 `assetName`: A file in the repo.
-  <i style="color:gray;">(optional)</i> : This file or folder is optional and can be added or omitted as needed.

### Description of the respective folders

- 📁 `simulation-data` : *Contains all valuble data files of the asset.*
- 📁 `documentation` : *Contains an instruction as well as technical specification of the asset.*
- 📁 `metadata` :   *Contains all metadata which are necassary to describe this asset, that includes all domain sepcific metadata from the [Ontology Management Base Repository](https://github.com/GAIA-X4PLC-AAD/ontology-management-base) (and all GAIA-X metadata form the [gaia-x-compliant-claims-example](https://github.com/GAIA-X4PLC-AAD/gaia-x-compliant-claims-example) to be compliant with the [GAIA-X Trust Framework](https://docs.gaia-x.eu/policy-rules-committee/trust-framework/22.10/). -> needs to be defined in a next step)*
- 📁 `validation-reports` :   *Contains the results provided by a validation suite.*
- 📁 `media` : *Contains all viusalization content from the asset which includes positionings decribed by a bounding box or maps as well as images and videos.*

### Description of the respective files

📄 `manifest_reference.json`:

- *This manifest file defined the link structure depending on the domain sepecific asset.zip. It includes a context section defining namespaces for various terms, an identifier (`@id`) for the asset, and a type (`@type`) indicating it is a manifest. The `manifest:links` section contains multiple entries, each specifying a type of link (e.g., license, simulation-data, media) with details such as relative paths, formats, and access roles. Optional metadata and visualization files are also included, with different access roles like `isOwner`,`isRegistered`, and `isPublic`.*

📄 `environment-model_instance.json` (domain metadata):

- *This JSON file describes the metadata and links associated with an environment-model used in the Gaia-X 4 PLC-AAD project. It includes a context section defining namespaces for various terms, an identifier (@id) for the environment-model, and a type (@type) indicating it is an environment-model SimulationAsset. The `DataResource` section provides details such as the name, description, and the GAIA-X metadata from the [gaia-x-compliant-claims-example](https://github.com/GAIA-X4PLC-AAD/gaia-x-compliant-claims-example) to be compliant with the [GAIA-X Trust Framework](https://docs.gaia-x.eu/policy-rules-committee/trust-framework/22.10/). The `manifest` section contains multiple entries, each specified by a category of link (e.g., simulation-data, metadata, media, documentation, validation-report) with details such as URLs and types. The `format` section specifies the type and version of the environment-model format. The `content` section describes road types, lane types, and traffic direction. The `quantity` section provides measurements like length, elevation range, and counts of intersections, traffic lights, and signs. The `quality` section details precision and accuracy metrics. The `dataSource` section lists the data sources and measurement system used. Finally, the `georeference` section provides geolocation information, including the bounding box and geodetic reference system.*

### Create an asset

You can use the GaiaX 4 PLC-AAD [Provider Services](https://github.com/GAIA-X4PLC-AAD/provider-services) and [Provider Tools](https://github.com/GAIA-X4PLC-AAD/provider-tools) to create your own digital asset.
