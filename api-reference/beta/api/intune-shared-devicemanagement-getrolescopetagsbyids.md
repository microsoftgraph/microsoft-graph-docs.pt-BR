---
title: função Funçãogetrolescopetagsbyids
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a63e3f1defaa5a0be7f650424bd8a111fb468cbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085588"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="850ed-103">função Funçãogetrolescopetagsbyids</span><span class="sxs-lookup"><span data-stu-id="850ed-103">getRoleScopeTagsByIds function</span></span>

<span data-ttu-id="850ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="850ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="850ed-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="850ed-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="850ed-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="850ed-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="850ed-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="850ed-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="850ed-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="850ed-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="850ed-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="850ed-109">Prerequisites</span></span>
<span data-ttu-id="850ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="850ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="850ed-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="850ed-112">Permission type</span></span>|<span data-ttu-id="850ed-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="850ed-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="850ed-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="850ed-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="850ed-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="850ed-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="850ed-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="850ed-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="850ed-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="850ed-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="850ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="850ed-118">Not supported.</span></span>|
|<span data-ttu-id="850ed-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="850ed-119">Application</span></span>||
| <span data-ttu-id="850ed-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="850ed-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="850ed-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="850ed-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="850ed-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="850ed-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="850ed-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="850ed-123">Request headers</span></span>
|<span data-ttu-id="850ed-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="850ed-124">Header</span></span>|<span data-ttu-id="850ed-125">Valor</span><span class="sxs-lookup"><span data-stu-id="850ed-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="850ed-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="850ed-126">Authorization</span></span>|<span data-ttu-id="850ed-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="850ed-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="850ed-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="850ed-128">Accept</span></span>|<span data-ttu-id="850ed-129">application/json</span><span class="sxs-lookup"><span data-stu-id="850ed-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="850ed-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="850ed-130">Request body</span></span>
<span data-ttu-id="850ed-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="850ed-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="850ed-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="850ed-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="850ed-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="850ed-133">Property</span></span>|<span data-ttu-id="850ed-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="850ed-134">Type</span></span>|<span data-ttu-id="850ed-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="850ed-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="850ed-136">ids</span><span class="sxs-lookup"><span data-stu-id="850ed-136">ids</span></span>|<span data-ttu-id="850ed-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="850ed-137">String collection</span></span>|<span data-ttu-id="850ed-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="850ed-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="850ed-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="850ed-139">Response</span></span>
<span data-ttu-id="850ed-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="850ed-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="850ed-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="850ed-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="850ed-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="850ed-142">Request</span></span>
<span data-ttu-id="850ed-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="850ed-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="850ed-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="850ed-144">Response</span></span>
<span data-ttu-id="850ed-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="850ed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```












