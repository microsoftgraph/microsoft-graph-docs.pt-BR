---
title: ação createMigrationReport
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44ad61c031c61033b07876973126f6569a81eaaf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535804"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="4f4fd-103">ação createMigrationReport</span><span class="sxs-lookup"><span data-stu-id="4f4fd-103">createMigrationReport action</span></span>

> <span data-ttu-id="4f4fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f4fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f4fd-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4f4fd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f4fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f4fd-107">Prerequisites</span></span>
<span data-ttu-id="4f4fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f4fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f4fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f4fd-110">Permission type</span></span>|<span data-ttu-id="4f4fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f4fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f4fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f4fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f4fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f4fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f4fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f4fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-115">Not supported.</span></span>|
|<span data-ttu-id="4f4fd-116">Application</span><span class="sxs-lookup"><span data-stu-id="4f4fd-116">Application</span></span>|<span data-ttu-id="4f4fd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4fd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f4fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f4fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="4f4fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f4fd-119">Request headers</span></span>
|<span data-ttu-id="4f4fd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f4fd-120">Header</span></span>|<span data-ttu-id="4f4fd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f4fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f4fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f4fd-122">Authorization</span></span>|<span data-ttu-id="4f4fd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f4fd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f4fd-124">Accept</span></span>|<span data-ttu-id="4f4fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f4fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f4fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f4fd-126">Request body</span></span>
<span data-ttu-id="4f4fd-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4f4fd-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4f4fd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f4fd-129">Property</span></span>|<span data-ttu-id="4f4fd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f4fd-130">Type</span></span>|<span data-ttu-id="4f4fd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f4fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f4fd-132">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="4f4fd-132">groupPolicyObjectFile</span></span>|[<span data-ttu-id="4f4fd-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="4f4fd-133">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="4f4fd-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4f4fd-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f4fd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f4fd-135">Response</span></span>
<span data-ttu-id="4f4fd-136">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f4fd-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f4fd-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f4fd-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f4fd-138">Request</span></span>
<span data-ttu-id="4f4fd-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/createMigrationReport

Content-type: application/json
Content-length: 191

{
  "groupPolicyObjectFile": {
    "@odata.type": "microsoft.graph.groupPolicyObjectFile",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "content": "Content value"
  }
}
```

### <a name="response"></a><span data-ttu-id="4f4fd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f4fd-140">Response</span></span>
<span data-ttu-id="4f4fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f4fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```






