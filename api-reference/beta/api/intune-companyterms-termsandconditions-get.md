---
title: Acessar termsAndConditions
description: Leia as propriedades e as relações do objeto termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9565671a5efd00fd0b6d5fbd859f68b0d0bc16de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933890"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="306cb-103">Acessar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="306cb-103">Get termsAndConditions</span></span>

> <span data-ttu-id="306cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="306cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="306cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="306cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="306cb-106">Leia as propriedades e as relações do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="306cb-106">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="306cb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="306cb-107">Prerequisites</span></span>
<span data-ttu-id="306cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="306cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="306cb-110">Permission type</span></span>|<span data-ttu-id="306cb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="306cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="306cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="306cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="306cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="306cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="306cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="306cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="306cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="306cb-115">Not supported.</span></span>|
|<span data-ttu-id="306cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="306cb-116">Application</span></span>|<span data-ttu-id="306cb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="306cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="306cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="306cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="306cb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="306cb-119">Optional query parameters</span></span>
<span data-ttu-id="306cb-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="306cb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="306cb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="306cb-121">Request headers</span></span>
|<span data-ttu-id="306cb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="306cb-122">Header</span></span>|<span data-ttu-id="306cb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="306cb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="306cb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="306cb-124">Authorization</span></span>|<span data-ttu-id="306cb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="306cb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="306cb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="306cb-126">Accept</span></span>|<span data-ttu-id="306cb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="306cb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="306cb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="306cb-128">Request body</span></span>
<span data-ttu-id="306cb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="306cb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="306cb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="306cb-130">Response</span></span>
<span data-ttu-id="306cb-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="306cb-131">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="306cb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="306cb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="306cb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="306cb-133">Request</span></span>
<span data-ttu-id="306cb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="306cb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="306cb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="306cb-135">Response</span></span>
<span data-ttu-id="306cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="306cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```




