---
title: Acessar termsAndConditions
description: Leia as propriedades e as relações do objeto termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f741df8ff5e244f2c90e86d5cd50ed633dfcf08
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244007"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="011c7-103">Acessar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="011c7-103">Get termsAndConditions</span></span>

<span data-ttu-id="011c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="011c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="011c7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="011c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="011c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="011c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="011c7-107">Leia as propriedades e as relações do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="011c7-107">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="011c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="011c7-108">Prerequisites</span></span>
<span data-ttu-id="011c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="011c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="011c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="011c7-111">Permission type</span></span>|<span data-ttu-id="011c7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="011c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="011c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="011c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="011c7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="011c7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="011c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="011c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="011c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="011c7-116">Not supported.</span></span>|
|<span data-ttu-id="011c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="011c7-117">Application</span></span>|<span data-ttu-id="011c7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="011c7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="011c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="011c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="011c7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="011c7-120">Optional query parameters</span></span>
<span data-ttu-id="011c7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="011c7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="011c7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="011c7-122">Request headers</span></span>
|<span data-ttu-id="011c7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="011c7-123">Header</span></span>|<span data-ttu-id="011c7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="011c7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="011c7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="011c7-125">Authorization</span></span>|<span data-ttu-id="011c7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="011c7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="011c7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="011c7-127">Accept</span></span>|<span data-ttu-id="011c7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="011c7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="011c7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="011c7-129">Request body</span></span>
<span data-ttu-id="011c7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="011c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="011c7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="011c7-131">Response</span></span>
<span data-ttu-id="011c7-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="011c7-132">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="011c7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="011c7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="011c7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="011c7-134">Request</span></span>
<span data-ttu-id="011c7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="011c7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="011c7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="011c7-136">Response</span></span>
<span data-ttu-id="011c7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="011c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

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
    "version": 7,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




