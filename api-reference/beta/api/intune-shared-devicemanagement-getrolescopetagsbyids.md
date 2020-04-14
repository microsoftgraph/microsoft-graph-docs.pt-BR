---
title: função Funçãogetrolescopetagsbyids
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57532f6eaf9f4ba8a6dfa4efe37930e3121bc8cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390134"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="6434d-103">função Funçãogetrolescopetagsbyids</span><span class="sxs-lookup"><span data-stu-id="6434d-103">getRoleScopeTagsByIds function</span></span>

<span data-ttu-id="6434d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6434d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6434d-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6434d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6434d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6434d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6434d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6434d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6434d-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6434d-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6434d-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6434d-109">Prerequisites</span></span>
<span data-ttu-id="6434d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6434d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6434d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6434d-112">Permission type</span></span>|<span data-ttu-id="6434d-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6434d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6434d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6434d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6434d-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6434d-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6434d-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6434d-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6434d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6434d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6434d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6434d-118">Not supported.</span></span>|
|<span data-ttu-id="6434d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6434d-119">Application</span></span>||
| <span data-ttu-id="6434d-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6434d-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6434d-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6434d-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6434d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6434d-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="6434d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6434d-123">Request headers</span></span>
|<span data-ttu-id="6434d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6434d-124">Header</span></span>|<span data-ttu-id="6434d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6434d-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6434d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6434d-126">Authorization</span></span>|<span data-ttu-id="6434d-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6434d-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6434d-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6434d-128">Accept</span></span>|<span data-ttu-id="6434d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6434d-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6434d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6434d-130">Request body</span></span>
<span data-ttu-id="6434d-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="6434d-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6434d-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="6434d-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6434d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6434d-133">Property</span></span>|<span data-ttu-id="6434d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6434d-134">Type</span></span>|<span data-ttu-id="6434d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6434d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6434d-136">ids</span><span class="sxs-lookup"><span data-stu-id="6434d-136">ids</span></span>|<span data-ttu-id="6434d-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6434d-137">String collection</span></span>|<span data-ttu-id="6434d-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6434d-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6434d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6434d-139">Response</span></span>
<span data-ttu-id="6434d-140">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6434d-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6434d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6434d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6434d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6434d-142">Request</span></span>
<span data-ttu-id="6434d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6434d-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="6434d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6434d-144">Response</span></span>
<span data-ttu-id="6434d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6434d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









