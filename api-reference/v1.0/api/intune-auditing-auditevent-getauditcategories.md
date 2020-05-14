---
title: Função getAuditCategories
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7c8b4e9ec640798e01cf2b92ec85a3a2cce5150
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43470504"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="fcd3f-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="fcd3f-103">getAuditCategories function</span></span>

<span data-ttu-id="fcd3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcd3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcd3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcd3f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcd3f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcd3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcd3f-107">Prerequisites</span></span>
<span data-ttu-id="fcd3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcd3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcd3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcd3f-110">Permission type</span></span>|<span data-ttu-id="fcd3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fcd3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcd3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcd3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fcd3f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd3f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fcd3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcd3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcd3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-115">Not supported.</span></span>|
|<span data-ttu-id="fcd3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcd3f-116">Application</span></span>|<span data-ttu-id="fcd3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcd3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcd3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="fcd3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd3f-119">Request headers</span></span>
|<span data-ttu-id="fcd3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcd3f-120">Header</span></span>|<span data-ttu-id="fcd3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fcd3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcd3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcd3f-122">Authorization</span></span>|<span data-ttu-id="fcd3f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcd3f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcd3f-124">Accept</span></span>|<span data-ttu-id="fcd3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fcd3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcd3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd3f-126">Request body</span></span>
<span data-ttu-id="fcd3f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcd3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcd3f-128">Response</span></span>
<span data-ttu-id="fcd3f-129">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcd3f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcd3f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcd3f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd3f-131">Request</span></span>
<span data-ttu-id="fcd3f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="fcd3f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcd3f-133">Response</span></span>
<span data-ttu-id="fcd3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcd3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```






