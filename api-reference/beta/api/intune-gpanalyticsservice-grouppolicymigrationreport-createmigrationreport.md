---
title: ação createMigrationReport
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e4aef4926934673586391cebffdf9156e257fe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465503"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="1e740-103">ação createMigrationReport</span><span class="sxs-lookup"><span data-stu-id="1e740-103">createMigrationReport action</span></span>

<span data-ttu-id="1e740-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1e740-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e740-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e740-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e740-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e740-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e740-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e740-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e740-108">Prerequisites</span></span>
<span data-ttu-id="1e740-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e740-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e740-111">Permission type</span></span>|<span data-ttu-id="1e740-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e740-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e740-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e740-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e740-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e740-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e740-116">Not supported.</span></span>|
|<span data-ttu-id="1e740-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e740-117">Application</span></span>|<span data-ttu-id="1e740-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e740-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e740-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="1e740-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-120">Request headers</span></span>
|<span data-ttu-id="1e740-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e740-121">Header</span></span>|<span data-ttu-id="1e740-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e740-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e740-123">Authorization</span></span>|<span data-ttu-id="1e740-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e740-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e740-125">Accept</span></span>|<span data-ttu-id="1e740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e740-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-127">Request body</span></span>
<span data-ttu-id="1e740-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1e740-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1e740-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1e740-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1e740-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e740-130">Property</span></span>|<span data-ttu-id="1e740-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e740-131">Type</span></span>|<span data-ttu-id="1e740-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e740-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="1e740-133">groupPolicyObjectFile</span></span>|[<span data-ttu-id="1e740-134">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="1e740-134">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="1e740-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e740-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1e740-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e740-136">Response</span></span>
<span data-ttu-id="1e740-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e740-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e740-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e740-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e740-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-139">Request</span></span>
<span data-ttu-id="1e740-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e740-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e740-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e740-141">Response</span></span>
<span data-ttu-id="1e740-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e740-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```





