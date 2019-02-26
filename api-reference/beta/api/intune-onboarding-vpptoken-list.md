---
title: Listar vppTokens
description: Listar propriedades e relações de objetos vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f10f196912448a591d6a96559b58dec6bf4b322a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144979"
---
# <a name="list-vpptokens"></a><span data-ttu-id="bc24e-103">Listar vppTokens</span><span class="sxs-lookup"><span data-stu-id="bc24e-103">List vppTokens</span></span>

> <span data-ttu-id="bc24e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc24e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc24e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc24e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc24e-106">Lista propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="bc24e-106">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc24e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc24e-107">Prerequisites</span></span>
<span data-ttu-id="bc24e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc24e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc24e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc24e-110">Permission type</span></span>|<span data-ttu-id="bc24e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc24e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc24e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc24e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc24e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc24e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="bc24e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc24e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc24e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc24e-115">Not supported.</span></span>|
|<span data-ttu-id="bc24e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc24e-116">Application</span></span>|<span data-ttu-id="bc24e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc24e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc24e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc24e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="bc24e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc24e-119">Request headers</span></span>
|<span data-ttu-id="bc24e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc24e-120">Header</span></span>|<span data-ttu-id="bc24e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc24e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc24e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc24e-122">Authorization</span></span>|<span data-ttu-id="bc24e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc24e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc24e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc24e-124">Accept</span></span>|<span data-ttu-id="bc24e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc24e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc24e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc24e-126">Request body</span></span>
<span data-ttu-id="bc24e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc24e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc24e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc24e-128">Response</span></span>
<span data-ttu-id="bc24e-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc24e-129">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc24e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc24e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc24e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc24e-131">Request</span></span>
<span data-ttu-id="bc24e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc24e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="bc24e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc24e-133">Response</span></span>
<span data-ttu-id="bc24e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc24e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1264

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
      "tokenActionResults": [
        {
          "@odata.type": "microsoft.graph.vppTokenActionResult",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ],
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value",
      "dataSharingConsentGranted": true,
      "displayName": "Display Name value",
      "locationName": "Location Name value",
      "claimTokenManagementFromExternalMdm": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




