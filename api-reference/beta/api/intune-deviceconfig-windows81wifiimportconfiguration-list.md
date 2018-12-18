---
title: Lista windows81WifiImportConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windows81WifiImportConfiguration.
author: tfitzmac
ms.openlocfilehash: 144c78fd00ad46702b6a042d2d11018498325cc3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313962"
---
# <a name="list-windows81wifiimportconfigurations"></a><span data-ttu-id="c7f41-103">Lista windows81WifiImportConfigurations</span><span class="sxs-lookup"><span data-stu-id="c7f41-103">List windows81WifiImportConfigurations</span></span>

> <span data-ttu-id="c7f41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7f41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7f41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7f41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7f41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7f41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7f41-107">Lista as propriedades e os relacionamentos dos objetos [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7f41-107">List properties and relationships of the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7f41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7f41-108">Prerequisites</span></span>
<span data-ttu-id="c7f41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7f41-111">Permission type</span></span>|<span data-ttu-id="c7f41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7f41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7f41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7f41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7f41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7f41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7f41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7f41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7f41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7f41-116">Not supported.</span></span>|
|<span data-ttu-id="c7f41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7f41-117">Application</span></span>|<span data-ttu-id="c7f41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7f41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7f41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7f41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f41-120">Request headers</span></span>
|<span data-ttu-id="c7f41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7f41-121">Header</span></span>|<span data-ttu-id="c7f41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7f41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7f41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7f41-123">Authorization</span></span>|<span data-ttu-id="c7f41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7f41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7f41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7f41-125">Accept</span></span>|<span data-ttu-id="c7f41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7f41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f41-127">Request body</span></span>
<span data-ttu-id="c7f41-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7f41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f41-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7f41-129">Response</span></span>
<span data-ttu-id="c7f41-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f41-130">If successful, this method returns a `200 OK` response code and a collection of [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7f41-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7f41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7f41-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f41-132">Request</span></span>
<span data-ttu-id="c7f41-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7f41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c7f41-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7f41-134">Response</span></span>
<span data-ttu-id="c7f41-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7f41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 642

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
      "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadFileName": "Payload File Name value",
      "profileName": "Profile Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```





