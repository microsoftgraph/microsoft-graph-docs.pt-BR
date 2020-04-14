---
title: Obter importedDeviceIdentityResult
description: Leia as propriedades e as relações do objeto importedDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80b1d4d1384294225838a9af83e8df67952948de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450980"
---
# <a name="get-importeddeviceidentityresult"></a><span data-ttu-id="44ac4-103">Obter importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="44ac4-103">Get importedDeviceIdentityResult</span></span>

<span data-ttu-id="44ac4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44ac4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44ac4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44ac4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ac4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44ac4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ac4-107">Leia as propriedades e as relações do objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="44ac4-107">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44ac4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44ac4-108">Prerequisites</span></span>
<span data-ttu-id="44ac4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ac4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44ac4-111">Permission type</span></span>|<span data-ttu-id="44ac4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44ac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ac4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44ac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44ac4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44ac4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="44ac4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44ac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44ac4-116">Not supported.</span></span>|
|<span data-ttu-id="44ac4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44ac4-117">Application</span></span>|<span data-ttu-id="44ac4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44ac4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ac4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44ac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44ac4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44ac4-120">Optional query parameters</span></span>
<span data-ttu-id="44ac4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44ac4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44ac4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44ac4-122">Request headers</span></span>
|<span data-ttu-id="44ac4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44ac4-123">Header</span></span>|<span data-ttu-id="44ac4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="44ac4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ac4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="44ac4-125">Authorization</span></span>|<span data-ttu-id="44ac4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44ac4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ac4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44ac4-127">Accept</span></span>|<span data-ttu-id="44ac4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="44ac4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ac4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44ac4-129">Request body</span></span>
<span data-ttu-id="44ac4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44ac4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44ac4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ac4-131">Response</span></span>
<span data-ttu-id="44ac4-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44ac4-132">If successful, this method returns a `200 OK` response code and [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ac4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44ac4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="44ac4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44ac4-134">Request</span></span>
<span data-ttu-id="44ac4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44ac4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="44ac4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ac4-136">Response</span></span>
<span data-ttu-id="44ac4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44ac4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": {
    "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
    "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
    "importedDeviceIdentifier": "Imported Device Identifier value",
    "importedDeviceIdentityType": "imei",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "description": "Description value",
    "enrollmentState": "enrolled",
    "platform": "ios",
    "status": true
  }
}
```



