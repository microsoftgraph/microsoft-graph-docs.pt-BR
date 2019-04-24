---
title: Listar iosCustomConfigurations
description: Listar propriedades e relações dos objetos iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c7a418e2e61dd4aeb4bc8e5feac1e053379b82c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467551"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="57666-103">Listar iosCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="57666-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="57666-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57666-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57666-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57666-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57666-106">Listar propriedades e relações dos objetos [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57666-106">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57666-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57666-107">Prerequisites</span></span>
<span data-ttu-id="57666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57666-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57666-110">Permission type</span></span>|<span data-ttu-id="57666-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57666-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57666-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57666-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57666-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57666-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57666-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57666-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57666-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57666-115">Not supported.</span></span>|
|<span data-ttu-id="57666-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57666-116">Application</span></span>|<span data-ttu-id="57666-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57666-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57666-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57666-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57666-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57666-119">Request headers</span></span>
|<span data-ttu-id="57666-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57666-120">Header</span></span>|<span data-ttu-id="57666-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57666-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57666-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57666-122">Authorization</span></span>|<span data-ttu-id="57666-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57666-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57666-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57666-124">Accept</span></span>|<span data-ttu-id="57666-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57666-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57666-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57666-126">Request body</span></span>
<span data-ttu-id="57666-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57666-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57666-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57666-128">Response</span></span>
<span data-ttu-id="57666-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57666-129">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57666-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57666-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="57666-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57666-131">Request</span></span>
<span data-ttu-id="57666-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57666-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="57666-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="57666-133">Response</span></span>
<span data-ttu-id="57666-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57666-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```





