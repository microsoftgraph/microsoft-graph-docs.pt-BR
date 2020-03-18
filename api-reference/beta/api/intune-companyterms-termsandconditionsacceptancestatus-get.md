---
title: Get termsAndConditionsAcceptanceStatus
description: Ler propriedades e relações do objeto termsAndConditionsAcceptanceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1736789afc589e2ece44a7fa56a283b24d71219
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760127"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="ecf15-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ecf15-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="ecf15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecf15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecf15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecf15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecf15-106">Ler propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ecf15-106">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecf15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecf15-107">Prerequisites</span></span>
<span data-ttu-id="ecf15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecf15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecf15-110">Permission type</span></span>|<span data-ttu-id="ecf15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecf15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecf15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecf15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecf15-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecf15-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ecf15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecf15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecf15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecf15-115">Not supported.</span></span>|
|<span data-ttu-id="ecf15-116">Application</span><span class="sxs-lookup"><span data-stu-id="ecf15-116">Application</span></span>|<span data-ttu-id="ecf15-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecf15-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecf15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecf15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecf15-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecf15-119">Optional query parameters</span></span>
<span data-ttu-id="ecf15-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecf15-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecf15-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf15-121">Request headers</span></span>
|<span data-ttu-id="ecf15-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecf15-122">Header</span></span>|<span data-ttu-id="ecf15-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ecf15-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecf15-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecf15-124">Authorization</span></span>|<span data-ttu-id="ecf15-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecf15-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecf15-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecf15-126">Accept</span></span>|<span data-ttu-id="ecf15-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ecf15-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecf15-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf15-128">Request body</span></span>
<span data-ttu-id="ecf15-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecf15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecf15-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf15-130">Response</span></span>
<span data-ttu-id="ecf15-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecf15-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf15-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecf15-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecf15-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf15-133">Request</span></span>
<span data-ttu-id="ecf15-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecf15-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="ecf15-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf15-135">Response</span></span>
<span data-ttu-id="ecf15-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecf15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




