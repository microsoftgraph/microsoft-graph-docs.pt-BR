---
title: Listar vppTokens
description: Listar propriedades e relações de objetos vppToken.
author: tfitzmac
ms.openlocfilehash: 8ecb087ac8d1cca8362128d429f6b1eff232dc46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311512"
---
# <a name="list-vpptokens"></a><span data-ttu-id="09f8d-103">Listar vppTokens</span><span class="sxs-lookup"><span data-stu-id="09f8d-103">List vppTokens</span></span>

> <span data-ttu-id="09f8d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="09f8d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09f8d-105">Lista propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="09f8d-105">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09f8d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09f8d-106">Prerequisites</span></span>
<span data-ttu-id="09f8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09f8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09f8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09f8d-109">Permission type</span></span>|<span data-ttu-id="09f8d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09f8d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09f8d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09f8d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09f8d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="09f8d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="09f8d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09f8d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09f8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09f8d-114">Not supported.</span></span>|
|<span data-ttu-id="09f8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09f8d-115">Application</span></span>|<span data-ttu-id="09f8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09f8d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09f8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09f8d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="09f8d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09f8d-118">Request headers</span></span>
|<span data-ttu-id="09f8d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09f8d-119">Header</span></span>|<span data-ttu-id="09f8d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="09f8d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09f8d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="09f8d-121">Authorization</span></span>|<span data-ttu-id="09f8d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09f8d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09f8d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="09f8d-123">Accept</span></span>|<span data-ttu-id="09f8d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09f8d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09f8d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09f8d-125">Request body</span></span>
<span data-ttu-id="09f8d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09f8d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09f8d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="09f8d-127">Response</span></span>
<span data-ttu-id="09f8d-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09f8d-128">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09f8d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09f8d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="09f8d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09f8d-130">Request</span></span>
<span data-ttu-id="09f8d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09f8d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="09f8d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="09f8d-132">Response</span></span>
<span data-ttu-id="09f8d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09f8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```



