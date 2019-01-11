---
title: Get androidForWorkSettings
description: Ler propriedades e relações do objeto androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bfc8b61cbb4e4074659eac660fd2b7dbfc700ddc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892257"
---
# <a name="get-androidforworksettings"></a><span data-ttu-id="c9214-103">Get androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="c9214-103">Get androidForWorkSettings</span></span>

> <span data-ttu-id="c9214-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9214-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9214-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9214-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9214-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c9214-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9214-107">Ler propriedades e relações do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="c9214-107">Read properties and relationships of the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9214-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9214-108">Prerequisites</span></span>
<span data-ttu-id="c9214-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9214-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9214-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9214-111">Permission type</span></span>|<span data-ttu-id="c9214-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9214-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9214-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9214-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9214-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9214-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9214-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9214-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9214-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9214-116">Not supported.</span></span>|
|<span data-ttu-id="c9214-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9214-117">Application</span></span>|<span data-ttu-id="c9214-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9214-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9214-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9214-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9214-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9214-120">Optional query parameters</span></span>
<span data-ttu-id="c9214-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9214-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9214-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9214-122">Request headers</span></span>
|<span data-ttu-id="c9214-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9214-123">Header</span></span>|<span data-ttu-id="c9214-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c9214-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9214-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9214-125">Authorization</span></span>|<span data-ttu-id="c9214-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9214-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9214-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9214-127">Accept</span></span>|<span data-ttu-id="c9214-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c9214-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9214-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9214-129">Request body</span></span>
<span data-ttu-id="c9214-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9214-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9214-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9214-131">Response</span></span>
<span data-ttu-id="c9214-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9214-132">If successful, this method returns a `200 OK` response code and [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9214-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9214-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9214-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9214-134">Request</span></span>
<span data-ttu-id="c9214-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9214-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
```

### <a name="response"></a><span data-ttu-id="c9214-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9214-136">Response</span></span>
<span data-ttu-id="c9214-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9214-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





