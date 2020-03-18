---
title: Get androidForWorkSettings
description: Ler propriedades e relações do objeto androidForWorkSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c92e744790228dc3e9018b8b2d1c887ab5b7138
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815674"
---
# <a name="get-androidforworksettings"></a><span data-ttu-id="e1cc9-103">Get androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="e1cc9-103">Get androidForWorkSettings</span></span>

> <span data-ttu-id="e1cc9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1cc9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1cc9-106">Ler propriedades e relações do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="e1cc9-106">Read properties and relationships of the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1cc9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1cc9-107">Prerequisites</span></span>
<span data-ttu-id="e1cc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1cc9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1cc9-110">Permission type</span></span>|<span data-ttu-id="e1cc9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1cc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1cc9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1cc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1cc9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1cc9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1cc9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1cc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1cc9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-115">Not supported.</span></span>|
|<span data-ttu-id="e1cc9-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1cc9-116">Application</span></span>|<span data-ttu-id="e1cc9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1cc9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1cc9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1cc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1cc9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1cc9-119">Optional query parameters</span></span>
<span data-ttu-id="e1cc9-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1cc9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1cc9-121">Request headers</span></span>
|<span data-ttu-id="e1cc9-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1cc9-122">Header</span></span>|<span data-ttu-id="e1cc9-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e1cc9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1cc9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1cc9-124">Authorization</span></span>|<span data-ttu-id="e1cc9-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1cc9-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1cc9-126">Accept</span></span>|<span data-ttu-id="e1cc9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1cc9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1cc9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1cc9-128">Request body</span></span>
<span data-ttu-id="e1cc9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1cc9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1cc9-130">Response</span></span>
<span data-ttu-id="e1cc9-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-131">If successful, this method returns a `200 OK` response code and [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1cc9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1cc9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1cc9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1cc9-133">Request</span></span>
<span data-ttu-id="e1cc9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
```

### <a name="response"></a><span data-ttu-id="e1cc9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1cc9-135">Response</span></span>
<span data-ttu-id="e1cc9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1cc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkSettings",
    "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true
  }
}
```




