# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="a8186-101">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a8186-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="a8186-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8186-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8186-103">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a8186-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="a8186-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8186-104">Properties</span></span>
|<span data-ttu-id="a8186-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8186-105">Property</span></span>|<span data-ttu-id="a8186-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8186-106">Type</span></span>|<span data-ttu-id="a8186-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8186-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8186-108">SubjectName</span><span class="sxs-lookup"><span data-stu-id="a8186-108">subjectName</span></span>|<span data-ttu-id="a8186-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8186-109">String</span></span>|<span data-ttu-id="a8186-110">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a8186-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="a8186-111">descrição</span><span class="sxs-lookup"><span data-stu-id="a8186-111">description</span></span>|<span data-ttu-id="a8186-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8186-112">String</span></span>|<span data-ttu-id="a8186-113">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a8186-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="a8186-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8186-114">expirationDateTime</span></span>|<span data-ttu-id="a8186-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8186-115">DateTimeOffset</span></span>|<span data-ttu-id="a8186-116">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a8186-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="a8186-117">certificado</span><span class="sxs-lookup"><span data-stu-id="a8186-117">certificate</span></span>|<span data-ttu-id="a8186-118">Binário</span><span class="sxs-lookup"><span data-stu-id="a8186-118">Binary</span></span>|<span data-ttu-id="a8186-119">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a8186-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8186-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a8186-120">Relationships</span></span>
<span data-ttu-id="a8186-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8186-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8186-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8186-122">JSON Representation</span></span>
<span data-ttu-id="a8186-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8186-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```








