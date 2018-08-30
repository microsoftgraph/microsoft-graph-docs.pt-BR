# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="91345-101">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91345-101">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="91345-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91345-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91345-103">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="91345-103">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="91345-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="91345-104">Methods</span></span>
|<span data-ttu-id="91345-105">Método</span><span class="sxs-lookup"><span data-stu-id="91345-105">Method</span></span>|<span data-ttu-id="91345-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="91345-106">Return Type</span></span>|<span data-ttu-id="91345-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="91345-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91345-108">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91345-108">Get applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_get.md)|[<span data-ttu-id="91345-109">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91345-109">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="91345-110">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="91345-110">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="91345-111">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91345-111">Update applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_update.md)|[<span data-ttu-id="91345-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91345-112">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="91345-113">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="91345-113">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="91345-114">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="91345-114">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="91345-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91345-115">String</span></span>|<span data-ttu-id="91345-116">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="91345-116">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="91345-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91345-117">Properties</span></span>
|<span data-ttu-id="91345-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91345-118">Property</span></span>|<span data-ttu-id="91345-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="91345-119">Type</span></span>|<span data-ttu-id="91345-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="91345-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91345-121">id</span><span class="sxs-lookup"><span data-stu-id="91345-121">id</span></span>|<span data-ttu-id="91345-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91345-122">String</span></span>|<span data-ttu-id="91345-123">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="91345-123">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="91345-124">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="91345-124">appleIdentifier</span></span>|<span data-ttu-id="91345-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91345-125">String</span></span>|<span data-ttu-id="91345-126">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="91345-126">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="91345-127">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="91345-127">topicIdentifier</span></span>|<span data-ttu-id="91345-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91345-128">String</span></span>|<span data-ttu-id="91345-129">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="91345-129">Topic Id.</span></span>|
|<span data-ttu-id="91345-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91345-130">lastModifiedDateTime</span></span>|<span data-ttu-id="91345-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91345-131">DateTimeOffset</span></span>|<span data-ttu-id="91345-132">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="91345-132">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="91345-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="91345-133">expirationDateTime</span></span>|<span data-ttu-id="91345-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91345-134">DateTimeOffset</span></span>|<span data-ttu-id="91345-135">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="91345-135">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="91345-136">certificado</span><span class="sxs-lookup"><span data-stu-id="91345-136">certificate</span></span>|<span data-ttu-id="91345-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91345-137">String</span></span>|<span data-ttu-id="91345-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="91345-138">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="91345-139">Relações</span><span class="sxs-lookup"><span data-stu-id="91345-139">Relationships</span></span>
<span data-ttu-id="91345-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91345-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91345-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91345-141">JSON Representation</span></span>
<span data-ttu-id="91345-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91345-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



