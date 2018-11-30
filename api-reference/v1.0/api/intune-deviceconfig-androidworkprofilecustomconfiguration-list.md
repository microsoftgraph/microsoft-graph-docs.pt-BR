---
title: Lista androidWorkProfileCustomConfigurations
description: Lista as propriedades e os relacionamentos dos objetos androidWorkProfileCustomConfiguration.
ms.openlocfilehash: 419cc4fa47e99691beb65dfbbf83c97df445cc4b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005206"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="52fd9-103">Lista androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="52fd9-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="52fd9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52fd9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52fd9-105">Lista as propriedades e os relacionamentos dos objetos [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52fd9-105">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52fd9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52fd9-106">Prerequisites</span></span>
<span data-ttu-id="52fd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52fd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52fd9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52fd9-109">Permission type</span></span>|<span data-ttu-id="52fd9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52fd9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52fd9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52fd9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52fd9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52fd9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52fd9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52fd9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52fd9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52fd9-114">Not supported.</span></span>|
|<span data-ttu-id="52fd9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52fd9-115">Application</span></span>|<span data-ttu-id="52fd9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52fd9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52fd9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52fd9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="52fd9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52fd9-118">Request headers</span></span>
|<span data-ttu-id="52fd9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52fd9-119">Header</span></span>|<span data-ttu-id="52fd9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="52fd9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52fd9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52fd9-121">Authorization</span></span>|<span data-ttu-id="52fd9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52fd9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52fd9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="52fd9-123">Accept</span></span>|<span data-ttu-id="52fd9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52fd9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52fd9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52fd9-125">Request body</span></span>
<span data-ttu-id="52fd9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52fd9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52fd9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="52fd9-127">Response</span></span>
<span data-ttu-id="52fd9-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52fd9-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52fd9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52fd9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="52fd9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52fd9-130">Request</span></span>
<span data-ttu-id="52fd9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52fd9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="52fd9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="52fd9-132">Response</span></span>
<span data-ttu-id="52fd9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52fd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```



