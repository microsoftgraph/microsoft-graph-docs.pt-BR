---
title: Ação validateFilter
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2315d4b42abd6289e77df767206197973e98fd3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160130"
---
# <a name="validatefilter-action"></a><span data-ttu-id="1bcc0-103">Ação validateFilter</span><span class="sxs-lookup"><span data-stu-id="1bcc0-103">validateFilter action</span></span>

<span data-ttu-id="1bcc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bcc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bcc0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bcc0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bcc0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bcc0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bcc0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bcc0-108">Prerequisites</span></span>
<span data-ttu-id="1bcc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bcc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bcc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bcc0-111">Permission type</span></span>|<span data-ttu-id="1bcc0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bcc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bcc0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bcc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bcc0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bcc0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bcc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bcc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bcc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-116">Not supported.</span></span>|
|<span data-ttu-id="1bcc0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bcc0-117">Application</span></span>|<span data-ttu-id="1bcc0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bcc0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bcc0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bcc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters/validateFilter
```

## <a name="request-headers"></a><span data-ttu-id="1bcc0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc0-120">Request headers</span></span>
|<span data-ttu-id="1bcc0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bcc0-121">Header</span></span>|<span data-ttu-id="1bcc0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bcc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bcc0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bcc0-123">Authorization</span></span>|<span data-ttu-id="1bcc0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bcc0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bcc0-125">Accept</span></span>|<span data-ttu-id="1bcc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bcc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bcc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc0-127">Request body</span></span>
<span data-ttu-id="1bcc0-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1bcc0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1bcc0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bcc0-130">Property</span></span>|<span data-ttu-id="1bcc0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bcc0-131">Type</span></span>|<span data-ttu-id="1bcc0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bcc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bcc0-133">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="1bcc0-133">deviceAndAppManagementAssignmentFilter</span></span>|[<span data-ttu-id="1bcc0-134">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="1bcc0-134">deviceAndAppManagementAssignmentFilter</span></span>](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|<span data-ttu-id="1bcc0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bcc0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1bcc0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcc0-136">Response</span></span>
<span data-ttu-id="1bcc0-137">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-137">If successful, this action returns a `200 OK` response code and a [assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bcc0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bcc0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bcc0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc0-139">Request</span></span>
<span data-ttu-id="1bcc0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/validateFilter

Content-type: application/json
Content-length: 520

{
  "deviceAndAppManagementAssignmentFilter": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
    "id": "819818db-18db-8198-db18-9881db189881",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "platform": "androidForWork",
    "rule": "Rule value",
    "roleScopeTags": [
      "Role Scope Tags value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="1bcc0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcc0-141">Response</span></span>
<span data-ttu-id="1bcc0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bcc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterValidationResult",
    "isValidRule": true
  }
}
```




