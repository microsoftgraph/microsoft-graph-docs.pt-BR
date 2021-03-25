---
title: Listar vppTokens
description: Lista propriedades e relações de objetos vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63057da7e78351c0bced2f7fdaf297c60f7c42f9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152658"
---
# <a name="list-vpptokens"></a><span data-ttu-id="60eed-103">Listar vppTokens</span><span class="sxs-lookup"><span data-stu-id="60eed-103">List vppTokens</span></span>

<span data-ttu-id="60eed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60eed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60eed-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60eed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60eed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60eed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60eed-107">Lista propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="60eed-107">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60eed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60eed-108">Prerequisites</span></span>
<span data-ttu-id="60eed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60eed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60eed-111">Permission type</span></span>|<span data-ttu-id="60eed-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60eed-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60eed-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60eed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60eed-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60eed-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="60eed-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60eed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60eed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60eed-116">Not supported.</span></span>|
|<span data-ttu-id="60eed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60eed-117">Application</span></span>|<span data-ttu-id="60eed-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60eed-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60eed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60eed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="60eed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60eed-120">Request headers</span></span>
|<span data-ttu-id="60eed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60eed-121">Header</span></span>|<span data-ttu-id="60eed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60eed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60eed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60eed-123">Authorization</span></span>|<span data-ttu-id="60eed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60eed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60eed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60eed-125">Accept</span></span>|<span data-ttu-id="60eed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60eed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60eed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60eed-127">Request body</span></span>
<span data-ttu-id="60eed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60eed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60eed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60eed-129">Response</span></span>
<span data-ttu-id="60eed-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60eed-130">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60eed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60eed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60eed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60eed-132">Request</span></span>
<span data-ttu-id="60eed-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60eed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="60eed-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="60eed-134">Response</span></span>
<span data-ttu-id="60eed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60eed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




