# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="4cb56-101">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4cb56-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="4cb56-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4cb56-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cb56-103">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="4cb56-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="4cb56-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cb56-104">Properties</span></span>
|<span data-ttu-id="4cb56-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cb56-105">Property</span></span>|<span data-ttu-id="4cb56-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cb56-106">Type</span></span>|<span data-ttu-id="4cb56-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cb56-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb56-108">SubjectName</span><span class="sxs-lookup"><span data-stu-id="4cb56-108">subjectName</span></span>|<span data-ttu-id="4cb56-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cb56-109">String</span></span>|<span data-ttu-id="4cb56-110">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4cb56-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="4cb56-111">descrição</span><span class="sxs-lookup"><span data-stu-id="4cb56-111">description</span></span>|<span data-ttu-id="4cb56-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cb56-112">String</span></span>|<span data-ttu-id="4cb56-113">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4cb56-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="4cb56-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb56-114">expirationDateTime</span></span>|<span data-ttu-id="4cb56-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb56-115">DateTimeOffset</span></span>|<span data-ttu-id="4cb56-116">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4cb56-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="4cb56-117">certificado</span><span class="sxs-lookup"><span data-stu-id="4cb56-117">ACS, certificate</span></span>|<span data-ttu-id="4cb56-118">Binário</span><span class="sxs-lookup"><span data-stu-id="4cb56-118">Binary</span></span>|<span data-ttu-id="4cb56-119">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4cb56-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cb56-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4cb56-120">Relationships</span></span>
<span data-ttu-id="4cb56-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cb56-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cb56-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cb56-122">JSON Representation</span></span>
<span data-ttu-id="4cb56-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cb56-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



