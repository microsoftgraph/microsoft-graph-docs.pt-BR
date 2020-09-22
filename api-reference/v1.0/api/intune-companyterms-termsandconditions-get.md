---
title: Acessar termsAndConditions
description: Leia as propriedades e as relações do objeto termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c47b66f3ec095e5e8e2716bfa6006a0188bdb923
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045905"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="c3919-103">Acessar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c3919-103">Get termsAndConditions</span></span>

<span data-ttu-id="c3919-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3919-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3919-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3919-106">Leia as propriedades e as relações do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="c3919-106">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3919-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3919-107">Prerequisites</span></span>
<span data-ttu-id="c3919-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3919-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3919-110">Permission type</span></span>|<span data-ttu-id="c3919-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3919-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3919-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3919-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3919-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3919-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c3919-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3919-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3919-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3919-115">Not supported.</span></span>|
|<span data-ttu-id="c3919-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3919-116">Application</span></span>|<span data-ttu-id="c3919-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3919-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3919-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3919-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3919-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3919-119">Optional query parameters</span></span>
<span data-ttu-id="c3919-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3919-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3919-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3919-121">Request headers</span></span>
|<span data-ttu-id="c3919-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3919-122">Header</span></span>|<span data-ttu-id="c3919-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c3919-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3919-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3919-124">Authorization</span></span>|<span data-ttu-id="c3919-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3919-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3919-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3919-126">Accept</span></span>|<span data-ttu-id="c3919-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3919-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3919-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3919-128">Request body</span></span>
<span data-ttu-id="c3919-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3919-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3919-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3919-130">Response</span></span>
<span data-ttu-id="c3919-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3919-131">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3919-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3919-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3919-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3919-133">Request</span></span>
<span data-ttu-id="c3919-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3919-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="c3919-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3919-135">Response</span></span>
<span data-ttu-id="c3919-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3919-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
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









