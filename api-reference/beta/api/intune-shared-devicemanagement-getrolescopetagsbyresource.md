---
title: Função getRoleScopeTagsByResource
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47742e8ea1611810bf36be8ca3c004c17b07425b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865940"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="a2fdb-103">Função getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="a2fdb-103">getRoleScopeTagsByResource function</span></span>

<span data-ttu-id="a2fdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2fdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2fdb-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2fdb-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2fdb-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2fdb-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a2fdb-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2fdb-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2fdb-109">Prerequisites</span></span>
<span data-ttu-id="a2fdb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2fdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2fdb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2fdb-112">Permission type</span></span>|<span data-ttu-id="a2fdb-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2fdb-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2fdb-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2fdb-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a2fdb-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="a2fdb-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="a2fdb-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2fdb-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a2fdb-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2fdb-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2fdb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-118">Not supported.</span></span>|
|<span data-ttu-id="a2fdb-119">Application</span><span class="sxs-lookup"><span data-stu-id="a2fdb-119">Application</span></span>||
| <span data-ttu-id="a2fdb-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="a2fdb-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="a2fdb-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2fdb-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2fdb-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2fdb-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="a2fdb-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fdb-123">Request headers</span></span>
|<span data-ttu-id="a2fdb-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2fdb-124">Header</span></span>|<span data-ttu-id="a2fdb-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a2fdb-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2fdb-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2fdb-126">Authorization</span></span>|<span data-ttu-id="a2fdb-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2fdb-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2fdb-128">Accept</span></span>|<span data-ttu-id="a2fdb-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a2fdb-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2fdb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fdb-130">Request body</span></span>
<span data-ttu-id="a2fdb-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a2fdb-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a2fdb-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2fdb-133">Property</span></span>|<span data-ttu-id="a2fdb-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2fdb-134">Type</span></span>|<span data-ttu-id="a2fdb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fdb-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2fdb-136">recurso</span><span class="sxs-lookup"><span data-stu-id="a2fdb-136">resource</span></span>|<span data-ttu-id="a2fdb-137">String</span><span class="sxs-lookup"><span data-stu-id="a2fdb-137">String</span></span>|<span data-ttu-id="a2fdb-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a2fdb-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2fdb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2fdb-139">Response</span></span>
<span data-ttu-id="a2fdb-140">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2fdb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2fdb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2fdb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fdb-142">Request</span></span>
<span data-ttu-id="a2fdb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a2fdb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2fdb-144">Response</span></span>
<span data-ttu-id="a2fdb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2fdb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










