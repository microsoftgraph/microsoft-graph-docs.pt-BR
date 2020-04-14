---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba8974a8785dcc922e14423410cf321b84442e85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454737"
---
# <a name="assign-action"></a><span data-ttu-id="b3075-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b3075-103">assign action</span></span>

<span data-ttu-id="b3075-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3075-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3075-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3075-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3075-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3075-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3075-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3075-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3075-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3075-108">Prerequisites</span></span>
<span data-ttu-id="b3075-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3075-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3075-111">Permission type</span></span>|<span data-ttu-id="b3075-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3075-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3075-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3075-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3075-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3075-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3075-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3075-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3075-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3075-116">Not supported.</span></span>|
|<span data-ttu-id="b3075-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3075-117">Application</span></span>|<span data-ttu-id="b3075-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3075-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3075-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3075-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b3075-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3075-120">Request headers</span></span>
|<span data-ttu-id="b3075-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3075-121">Header</span></span>|<span data-ttu-id="b3075-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3075-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3075-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3075-123">Authorization</span></span>|<span data-ttu-id="b3075-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3075-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3075-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3075-125">Accept</span></span>|<span data-ttu-id="b3075-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3075-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3075-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3075-127">Request body</span></span>
<span data-ttu-id="b3075-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b3075-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b3075-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b3075-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b3075-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3075-130">Property</span></span>|<span data-ttu-id="b3075-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3075-131">Type</span></span>|<span data-ttu-id="b3075-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3075-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3075-133">assignments</span><span class="sxs-lookup"><span data-stu-id="b3075-133">assignments</span></span>|<span data-ttu-id="b3075-134">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b3075-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b3075-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3075-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3075-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3075-136">Response</span></span>
<span data-ttu-id="b3075-137">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3075-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3075-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3075-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3075-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3075-139">Request</span></span>
<span data-ttu-id="b3075-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3075-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b3075-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3075-141">Response</span></span>
<span data-ttu-id="b3075-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3075-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



