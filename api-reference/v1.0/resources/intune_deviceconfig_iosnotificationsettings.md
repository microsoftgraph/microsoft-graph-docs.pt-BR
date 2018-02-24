# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="00376-101">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="00376-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="00376-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="00376-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00376-103">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="00376-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="00376-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00376-104">Properties</span></span>
|<span data-ttu-id="00376-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00376-105">Property</span></span>|<span data-ttu-id="00376-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="00376-106">Type</span></span>|<span data-ttu-id="00376-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="00376-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00376-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="00376-108">bundleID</span></span>|<span data-ttu-id="00376-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00376-109">String</span></span>|<span data-ttu-id="00376-110">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="00376-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="00376-111">appName</span><span class="sxs-lookup"><span data-stu-id="00376-111">appname</span></span>|<span data-ttu-id="00376-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00376-112">String</span></span>|<span data-ttu-id="00376-113">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="00376-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="00376-114">publicador</span><span class="sxs-lookup"><span data-stu-id="00376-114">Publisher</span></span>|<span data-ttu-id="00376-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00376-115">String</span></span>|<span data-ttu-id="00376-116">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="00376-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="00376-117">enabled</span><span class="sxs-lookup"><span data-stu-id="00376-117">enabled</span></span>|<span data-ttu-id="00376-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="00376-118">Boolean</span></span>|<span data-ttu-id="00376-119">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00376-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="00376-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="00376-120">showInNotificationCenter</span></span>|<span data-ttu-id="00376-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="00376-121">Boolean</span></span>|<span data-ttu-id="00376-122">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="00376-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="00376-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="00376-123">showOnLockScreen</span></span>|<span data-ttu-id="00376-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="00376-124">Boolean</span></span>|<span data-ttu-id="00376-125">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="00376-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="00376-126">alertType</span><span class="sxs-lookup"><span data-stu-id="00376-126">alertType</span></span>|<span data-ttu-id="00376-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00376-127">String</span></span>|<span data-ttu-id="00376-128">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00376-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="00376-129">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="00376-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="00376-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="00376-130">badgesEnabled</span></span>|<span data-ttu-id="00376-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="00376-131">Boolean</span></span>|<span data-ttu-id="00376-132">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00376-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="00376-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="00376-133">soundsEnabled</span></span>|<span data-ttu-id="00376-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="00376-134">Boolean</span></span>|<span data-ttu-id="00376-135">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00376-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00376-136">Relações</span><span class="sxs-lookup"><span data-stu-id="00376-136">Relationships</span></span>
<span data-ttu-id="00376-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00376-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00376-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00376-138">JSON Representation</span></span>
<span data-ttu-id="00376-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00376-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
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



