---
title: função Funçãogetrolescopetagsbyids
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b08e3af8741e66201076387ec37a6f018c84663a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735348"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="6d80e-103">função Funçãogetrolescopetagsbyids</span><span class="sxs-lookup"><span data-stu-id="6d80e-103">getRoleScopeTagsByIds function</span></span>

<span data-ttu-id="6d80e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d80e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d80e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d80e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d80e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d80e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d80e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d80e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d80e-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d80e-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d80e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d80e-109">Prerequisites</span></span>
<span data-ttu-id="6d80e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d80e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d80e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d80e-112">Permission type</span></span>|<span data-ttu-id="6d80e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d80e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d80e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d80e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6d80e-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6d80e-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6d80e-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d80e-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6d80e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d80e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d80e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d80e-118">Not supported.</span></span>|
|<span data-ttu-id="6d80e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d80e-119">Application</span></span>||
| <span data-ttu-id="6d80e-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6d80e-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6d80e-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d80e-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d80e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d80e-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="6d80e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d80e-123">Request headers</span></span>
|<span data-ttu-id="6d80e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d80e-124">Header</span></span>|<span data-ttu-id="6d80e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6d80e-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d80e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d80e-126">Authorization</span></span>|<span data-ttu-id="6d80e-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d80e-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d80e-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d80e-128">Accept</span></span>|<span data-ttu-id="6d80e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6d80e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d80e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d80e-130">Request body</span></span>
<span data-ttu-id="6d80e-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="6d80e-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6d80e-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="6d80e-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6d80e-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d80e-133">Property</span></span>|<span data-ttu-id="6d80e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d80e-134">Type</span></span>|<span data-ttu-id="6d80e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d80e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d80e-136">ids</span><span class="sxs-lookup"><span data-stu-id="6d80e-136">ids</span></span>|<span data-ttu-id="6d80e-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d80e-137">String collection</span></span>|<span data-ttu-id="6d80e-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d80e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d80e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d80e-139">Response</span></span>
<span data-ttu-id="6d80e-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d80e-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d80e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d80e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d80e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d80e-142">Request</span></span>
<span data-ttu-id="6d80e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d80e-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="6d80e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d80e-144">Response</span></span>
<span data-ttu-id="6d80e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d80e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











