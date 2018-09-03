# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="bde52-101">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="bde52-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="bde52-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bde52-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bde52-103">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="bde52-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="bde52-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bde52-104">Properties</span></span>
|<span data-ttu-id="bde52-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bde52-105">Property</span></span>|<span data-ttu-id="bde52-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="bde52-106">Type</span></span>|<span data-ttu-id="bde52-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="bde52-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bde52-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="bde52-108">bundleID</span></span>|<span data-ttu-id="bde52-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bde52-109">String</span></span>|<span data-ttu-id="bde52-110">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="bde52-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="bde52-111">appName</span><span class="sxs-lookup"><span data-stu-id="bde52-111">appName</span></span>|<span data-ttu-id="bde52-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bde52-112">String</span></span>|<span data-ttu-id="bde52-113">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="bde52-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="bde52-114">publicador</span><span class="sxs-lookup"><span data-stu-id="bde52-114">publisher</span></span>|<span data-ttu-id="bde52-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bde52-115">String</span></span>|<span data-ttu-id="bde52-116">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="bde52-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="bde52-117">enabled</span><span class="sxs-lookup"><span data-stu-id="bde52-117">enabled</span></span>|<span data-ttu-id="bde52-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="bde52-118">Boolean</span></span>|<span data-ttu-id="bde52-119">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bde52-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="bde52-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="bde52-120">showInNotificationCenter</span></span>|<span data-ttu-id="bde52-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="bde52-121">Boolean</span></span>|<span data-ttu-id="bde52-122">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="bde52-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="bde52-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="bde52-123">showOnLockScreen</span></span>|<span data-ttu-id="bde52-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="bde52-124">Boolean</span></span>|<span data-ttu-id="bde52-125">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="bde52-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="bde52-126">alertType</span><span class="sxs-lookup"><span data-stu-id="bde52-126">alertType</span></span>|[<span data-ttu-id="bde52-127">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="bde52-127">iosNotificationAlertType values</span></span>](../resources/intune_deviceconfig_iosnotificationalerttype.md)|<span data-ttu-id="bde52-128">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bde52-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="bde52-129">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="bde52-129">The possible values are `deviceDefault`, `banner`, `modal`, `none`, , , , , , , , or .</span></span>|
|<span data-ttu-id="bde52-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="bde52-130">badgesEnabled</span></span>|<span data-ttu-id="bde52-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="bde52-131">Boolean</span></span>|<span data-ttu-id="bde52-132">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bde52-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="bde52-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="bde52-133">soundsEnabled</span></span>|<span data-ttu-id="bde52-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="bde52-134">Boolean</span></span>|<span data-ttu-id="bde52-135">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bde52-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bde52-136">Relações</span><span class="sxs-lookup"><span data-stu-id="bde52-136">Relationships</span></span>
<span data-ttu-id="bde52-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bde52-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bde52-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bde52-138">JSON Representation</span></span>
<span data-ttu-id="bde52-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bde52-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



