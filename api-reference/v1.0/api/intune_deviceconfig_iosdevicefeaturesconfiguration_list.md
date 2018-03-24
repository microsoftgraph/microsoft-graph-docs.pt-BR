# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="786b4-101">Listar iosDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="786b4-101">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="786b4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="786b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="786b4-103">Listar propriedades e relações dos objetos [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="786b4-103">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="786b4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="786b4-104">Prerequisites</span></span>
<span data-ttu-id="786b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="786b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="786b4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="786b4-107">Permission type</span></span>|<span data-ttu-id="786b4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="786b4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="786b4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="786b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="786b4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="786b4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="786b4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="786b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="786b4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="786b4-112">Not supported.</span></span>|
|<span data-ttu-id="786b4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="786b4-113">Application</span></span>|<span data-ttu-id="786b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="786b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="786b4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="786b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="786b4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="786b4-116">Request headers</span></span>
|<span data-ttu-id="786b4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="786b4-117">Header</span></span>|<span data-ttu-id="786b4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="786b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="786b4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="786b4-119">Authorization</span></span>|<span data-ttu-id="786b4-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="786b4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="786b4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="786b4-121">Accept</span></span>|<span data-ttu-id="786b4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="786b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="786b4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="786b4-123">Request body</span></span>
<span data-ttu-id="786b4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="786b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786b4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="786b4-125">Response</span></span>
<span data-ttu-id="786b4-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786b4-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="786b4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="786b4-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="786b4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786b4-128">Request</span></span>
<span data-ttu-id="786b4-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786b4-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="786b4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="786b4-130">Response</span></span>
<span data-ttu-id="786b4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="786b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2461

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
      "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "assetTagTemplate": "Asset Tag Template value",
      "lockScreenFootnote": "Lock Screen Footnote value",
      "homeScreenDockIcons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ],
      "homeScreenPages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenPage",
          "displayName": "Display Name value",
          "icons": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolder",
              "displayName": "Display Name value",
              "pages": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                  "displayName": "Display Name value",
                  "apps": [
                    {
                      "@odata.type": "microsoft.graph.iosHomeScreenApp",
                      "displayName": "Display Name value",
                      "bundleID": "Bundle ID value"
                    }
                  ]
                }
              ]
            }
          ]
        }
      ],
      "notificationSettings": [
        {
          "@odata.type": "microsoft.graph.iosNotificationSettings",
          "bundleID": "Bundle ID value",
          "appName": "App Name value",
          "publisher": "Publisher value",
          "enabled": true,
          "showInNotificationCenter": true,
          "showOnLockScreen": true,
          "alertType": "banner",
          "badgesEnabled": true,
          "soundsEnabled": true
        }
      ]
    }
  ]
}
```



