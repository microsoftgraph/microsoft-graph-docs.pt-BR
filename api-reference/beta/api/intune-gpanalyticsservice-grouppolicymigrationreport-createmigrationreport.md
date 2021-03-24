---
title: Ação createMigrationReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f1be3e025a876cf4f702236386ff723497f550c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135569"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="ee5fb-103">Ação createMigrationReport</span><span class="sxs-lookup"><span data-stu-id="ee5fb-103">createMigrationReport action</span></span>

<span data-ttu-id="ee5fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee5fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee5fb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee5fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee5fb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee5fb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee5fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee5fb-108">Prerequisites</span></span>
<span data-ttu-id="ee5fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee5fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee5fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee5fb-111">Permission type</span></span>|<span data-ttu-id="ee5fb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee5fb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee5fb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee5fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee5fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee5fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee5fb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee5fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee5fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-116">Not supported.</span></span>|
|<span data-ttu-id="ee5fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee5fb-117">Application</span></span>|<span data-ttu-id="ee5fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee5fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee5fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee5fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="ee5fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5fb-120">Request headers</span></span>
|<span data-ttu-id="ee5fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee5fb-121">Header</span></span>|<span data-ttu-id="ee5fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee5fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee5fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee5fb-123">Authorization</span></span>|<span data-ttu-id="ee5fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee5fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee5fb-125">Accept</span></span>|<span data-ttu-id="ee5fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee5fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee5fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5fb-127">Request body</span></span>
<span data-ttu-id="ee5fb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee5fb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee5fb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee5fb-130">Property</span></span>|<span data-ttu-id="ee5fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee5fb-131">Type</span></span>|<span data-ttu-id="ee5fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee5fb-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="ee5fb-133">groupPolicyObjectFile</span></span>|[<span data-ttu-id="ee5fb-134">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="ee5fb-134">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="ee5fb-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee5fb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ee5fb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5fb-136">Response</span></span>
<span data-ttu-id="ee5fb-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee5fb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee5fb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee5fb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5fb-139">Request</span></span>
<span data-ttu-id="ee5fb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/createMigrationReport

Content-type: application/json
Content-length: 438

{
  "groupPolicyObjectFile": {
    "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
    "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "content": "Content value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ee5fb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5fb-141">Response</span></span>
<span data-ttu-id="ee5fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee5fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```




