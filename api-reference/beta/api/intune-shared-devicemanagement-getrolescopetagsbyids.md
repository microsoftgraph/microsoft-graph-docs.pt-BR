---
title: função Funçãogetrolescopetagsbyids
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40b228a59a426d09d760edb1490b890d91c69940
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538186"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="3b4f3-103">função Funçãogetrolescopetagsbyids</span><span class="sxs-lookup"><span data-stu-id="3b4f3-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="3b4f3-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b4f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b4f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b4f3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b4f3-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b4f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b4f3-108">Prerequisites</span></span>
<span data-ttu-id="3b4f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b4f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b4f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b4f3-111">Permission type</span></span>|<span data-ttu-id="3b4f3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b4f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b4f3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b4f3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3b4f3-114">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="3b4f3-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="3b4f3-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b4f3-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3b4f3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b4f3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b4f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-117">Not supported.</span></span>|
|<span data-ttu-id="3b4f3-118">Application</span><span class="sxs-lookup"><span data-stu-id="3b4f3-118">Application</span></span>||
| <span data-ttu-id="3b4f3-119">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="3b4f3-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="3b4f3-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b4f3-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b4f3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b4f3-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="3b4f3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b4f3-122">Request headers</span></span>
|<span data-ttu-id="3b4f3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b4f3-123">Header</span></span>|<span data-ttu-id="3b4f3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3b4f3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b4f3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b4f3-125">Authorization</span></span>|<span data-ttu-id="3b4f3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b4f3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b4f3-127">Accept</span></span>|<span data-ttu-id="3b4f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3b4f3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b4f3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b4f3-129">Request body</span></span>
<span data-ttu-id="3b4f3-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3b4f3-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3b4f3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b4f3-132">Property</span></span>|<span data-ttu-id="3b4f3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b4f3-133">Type</span></span>|<span data-ttu-id="3b4f3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b4f3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b4f3-135">ids</span><span class="sxs-lookup"><span data-stu-id="3b4f3-135">ids</span></span>|<span data-ttu-id="3b4f3-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b4f3-136">String collection</span></span>|<span data-ttu-id="3b4f3-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b4f3-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b4f3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b4f3-138">Response</span></span>
<span data-ttu-id="3b4f3-139">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b4f3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b4f3-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b4f3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b4f3-141">Request</span></span>
<span data-ttu-id="3b4f3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="3b4f3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b4f3-143">Response</span></span>
<span data-ttu-id="3b4f3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b4f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









