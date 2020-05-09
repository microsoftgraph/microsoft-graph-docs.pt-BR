---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1a91a55427f7c59aa912148e62aad23edb26a0a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177531"
---
# <a name="assign-action"></a><span data-ttu-id="aab45-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="aab45-103">assign action</span></span>

<span data-ttu-id="aab45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aab45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aab45-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aab45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aab45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aab45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aab45-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aab45-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aab45-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aab45-108">Prerequisites</span></span>
<span data-ttu-id="aab45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aab45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab45-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aab45-111">Permission type</span></span>|<span data-ttu-id="aab45-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aab45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab45-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aab45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aab45-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab45-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="aab45-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aab45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aab45-116">Not supported.</span></span>|
|<span data-ttu-id="aab45-117">Application</span><span class="sxs-lookup"><span data-stu-id="aab45-117">Application</span></span>|<span data-ttu-id="aab45-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab45-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab45-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aab45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/{roleScopeTagId}/assign
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="aab45-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aab45-120">Request headers</span></span>
|<span data-ttu-id="aab45-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aab45-121">Header</span></span>|<span data-ttu-id="aab45-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aab45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab45-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aab45-123">Authorization</span></span>|<span data-ttu-id="aab45-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aab45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab45-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aab45-125">Accept</span></span>|<span data-ttu-id="aab45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aab45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab45-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aab45-127">Request body</span></span>
<span data-ttu-id="aab45-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="aab45-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aab45-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="aab45-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aab45-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aab45-130">Property</span></span>|<span data-ttu-id="aab45-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aab45-131">Type</span></span>|<span data-ttu-id="aab45-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aab45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab45-133">assignments</span><span class="sxs-lookup"><span data-stu-id="aab45-133">assignments</span></span>|<span data-ttu-id="aab45-134">coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aab45-134">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="aab45-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aab45-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aab45-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aab45-136">Response</span></span>
<span data-ttu-id="aab45-137">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aab45-137">If successful, this action returns a `200 OK` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab45-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aab45-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="aab45-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aab45-139">Request</span></span>
<span data-ttu-id="aab45-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aab45-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}/assign

Content-type: application/json
Content-length: 262

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="aab45-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="aab45-141">Response</span></span>
<span data-ttu-id="aab45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aab45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



