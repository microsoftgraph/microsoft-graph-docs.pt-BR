---
title: Listar deviceConfigurationPolicySetItems
description: Listar propriedades e relações dos objetos deviceConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14f882b26cf0aaf8a1eafe028ad11407b88538b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156741"
---
# <a name="list-deviceconfigurationpolicysetitems"></a><span data-ttu-id="4ef53-103">Listar deviceConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="4ef53-103">List deviceConfigurationPolicySetItems</span></span>

<span data-ttu-id="4ef53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef53-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ef53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ef53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef53-107">Listar propriedades e relações dos [objetos deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ef53-107">List properties and relationships of the [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ef53-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ef53-108">Prerequisites</span></span>
<span data-ttu-id="4ef53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef53-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ef53-111">Permission type</span></span>|<span data-ttu-id="4ef53-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ef53-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ef53-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ef53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ef53-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef53-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ef53-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ef53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ef53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ef53-116">Not supported.</span></span>|
|<span data-ttu-id="4ef53-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ef53-117">Application</span></span>|<span data-ttu-id="4ef53-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef53-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ef53-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ef53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="4ef53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef53-120">Request headers</span></span>
|<span data-ttu-id="4ef53-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ef53-121">Header</span></span>|<span data-ttu-id="4ef53-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ef53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ef53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ef53-123">Authorization</span></span>|<span data-ttu-id="4ef53-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ef53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ef53-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ef53-125">Accept</span></span>|<span data-ttu-id="4ef53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ef53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef53-127">Request body</span></span>
<span data-ttu-id="4ef53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ef53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ef53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ef53-129">Response</span></span>
<span data-ttu-id="4ef53-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ef53-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef53-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ef53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ef53-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef53-132">Request</span></span>
<span data-ttu-id="4ef53-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ef53-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="4ef53-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ef53-134">Response</span></span>
<span data-ttu-id="4ef53-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ef53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
      "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```




