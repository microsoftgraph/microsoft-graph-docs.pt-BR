---
title: Função getAuditActivityTypes
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7e02ebe088be009acee817482674747e2e4b6c1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165601"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="379ae-103">Função getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="379ae-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="379ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="379ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="379ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="379ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="379ae-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="379ae-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="379ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="379ae-107">Prerequisites</span></span>
<span data-ttu-id="379ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="379ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="379ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="379ae-110">Permission type</span></span>|<span data-ttu-id="379ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="379ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="379ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="379ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="379ae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="379ae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="379ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="379ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="379ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="379ae-115">Not supported.</span></span>|
|<span data-ttu-id="379ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="379ae-116">Application</span></span>|<span data-ttu-id="379ae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="379ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="379ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="379ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="379ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="379ae-119">Request headers</span></span>
|<span data-ttu-id="379ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="379ae-120">Header</span></span>|<span data-ttu-id="379ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="379ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="379ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="379ae-122">Authorization</span></span>|<span data-ttu-id="379ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="379ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="379ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="379ae-124">Accept</span></span>|<span data-ttu-id="379ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="379ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="379ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="379ae-126">Request body</span></span>
<span data-ttu-id="379ae-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="379ae-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="379ae-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="379ae-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="379ae-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="379ae-129">Property</span></span>|<span data-ttu-id="379ae-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="379ae-130">Type</span></span>|<span data-ttu-id="379ae-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="379ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="379ae-132">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="379ae-132">category</span></span>|<span data-ttu-id="379ae-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="379ae-133">String</span></span>|<span data-ttu-id="379ae-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="379ae-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="379ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="379ae-135">Response</span></span>
<span data-ttu-id="379ae-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="379ae-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="379ae-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="379ae-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="379ae-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="379ae-138">Request</span></span>
<span data-ttu-id="379ae-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="379ae-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="379ae-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="379ae-140">Response</span></span>
<span data-ttu-id="379ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="379ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```




