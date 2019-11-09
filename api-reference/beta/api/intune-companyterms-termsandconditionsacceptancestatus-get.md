---
title: Get termsAndConditionsAcceptanceStatus
description: Ler propriedades e relações do objeto termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b4843c98561ac24e2c6213a41bb5cdc98aac8dc
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085068"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="8af38-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8af38-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="8af38-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8af38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8af38-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8af38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8af38-106">Ler propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8af38-106">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8af38-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8af38-107">Prerequisites</span></span>
<span data-ttu-id="8af38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8af38-110">Permission type</span></span>|<span data-ttu-id="8af38-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8af38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8af38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8af38-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8af38-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8af38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8af38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8af38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8af38-115">Not supported.</span></span>|
|<span data-ttu-id="8af38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8af38-116">Application</span></span>|<span data-ttu-id="8af38-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8af38-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8af38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8af38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8af38-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8af38-119">Optional query parameters</span></span>
<span data-ttu-id="8af38-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8af38-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8af38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8af38-121">Request headers</span></span>
|<span data-ttu-id="8af38-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8af38-122">Header</span></span>|<span data-ttu-id="8af38-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8af38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8af38-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8af38-124">Authorization</span></span>|<span data-ttu-id="8af38-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8af38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8af38-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8af38-126">Accept</span></span>|<span data-ttu-id="8af38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8af38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af38-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8af38-128">Request body</span></span>
<span data-ttu-id="8af38-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8af38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af38-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af38-130">Response</span></span>
<span data-ttu-id="8af38-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8af38-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af38-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8af38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8af38-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af38-133">Request</span></span>
<span data-ttu-id="8af38-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8af38-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="8af38-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af38-135">Response</span></span>
<span data-ttu-id="8af38-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8af38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```






