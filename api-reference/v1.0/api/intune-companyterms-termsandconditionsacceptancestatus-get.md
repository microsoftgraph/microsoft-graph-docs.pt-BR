---
title: Get termsAndConditionsAcceptanceStatus
description: Ler propriedades e relações do objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
ms.openlocfilehash: e5e2148a1b7adfa095f065dcc6a292657765d677
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311806"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="a50a7-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="a50a7-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="a50a7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a50a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a50a7-105">Ler propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a50a7-105">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a50a7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a50a7-106">Prerequisites</span></span>
<span data-ttu-id="a50a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a50a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a50a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a50a7-109">Permission type</span></span>|<span data-ttu-id="a50a7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a50a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a50a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a50a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a50a7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a50a7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a50a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a50a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a50a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a50a7-114">Not supported.</span></span>|
|<span data-ttu-id="a50a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a50a7-115">Application</span></span>|<span data-ttu-id="a50a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a50a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a50a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a50a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a50a7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a50a7-118">Optional query parameters</span></span>
<span data-ttu-id="a50a7-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a50a7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a50a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a50a7-120">Request headers</span></span>
|<span data-ttu-id="a50a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a50a7-121">Header</span></span>|<span data-ttu-id="a50a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a50a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a50a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a50a7-123">Authorization</span></span>|<span data-ttu-id="a50a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a50a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a50a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a50a7-125">Accept</span></span>|<span data-ttu-id="a50a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a50a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a50a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a50a7-127">Request body</span></span>
<span data-ttu-id="a50a7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a50a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a50a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a50a7-129">Response</span></span>
<span data-ttu-id="a50a7-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a50a7-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a50a7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a50a7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a50a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a50a7-132">Request</span></span>
<span data-ttu-id="a50a7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a50a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="a50a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a50a7-134">Response</span></span>
<span data-ttu-id="a50a7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a50a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



