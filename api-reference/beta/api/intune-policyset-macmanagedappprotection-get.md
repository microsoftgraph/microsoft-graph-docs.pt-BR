---
title: Obter macManagedAppProtection
description: Leia as propriedades e as relações do objeto macManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f85f6191516620140b26b99885b0af158516458
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191792"
---
# <a name="get-macmanagedappprotection"></a><span data-ttu-id="66976-103">Obter macManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="66976-103">Get macManagedAppProtection</span></span>

> <span data-ttu-id="66976-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66976-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66976-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66976-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66976-106">Leia as propriedades e as relações do objeto [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) .</span><span class="sxs-lookup"><span data-stu-id="66976-106">Read properties and relationships of the [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66976-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66976-107">Prerequisites</span></span>
<span data-ttu-id="66976-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66976-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66976-110">Permission type</span></span>|<span data-ttu-id="66976-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66976-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66976-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66976-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66976-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66976-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="66976-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66976-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66976-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66976-115">Not supported.</span></span>|
|<span data-ttu-id="66976-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66976-116">Application</span></span>|<span data-ttu-id="66976-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66976-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66976-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66976-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/macManagedAppProtections/{macManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66976-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66976-119">Optional query parameters</span></span>
<span data-ttu-id="66976-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66976-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66976-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66976-121">Request headers</span></span>
|<span data-ttu-id="66976-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66976-122">Header</span></span>|<span data-ttu-id="66976-123">Valor</span><span class="sxs-lookup"><span data-stu-id="66976-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66976-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="66976-124">Authorization</span></span>|<span data-ttu-id="66976-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66976-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66976-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66976-126">Accept</span></span>|<span data-ttu-id="66976-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66976-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66976-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66976-128">Request body</span></span>
<span data-ttu-id="66976-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66976-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66976-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="66976-130">Response</span></span>
<span data-ttu-id="66976-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66976-131">If successful, this method returns a `200 OK` response code and [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66976-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66976-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="66976-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66976-133">Request</span></span>
<span data-ttu-id="66976-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66976-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/macManagedAppProtections/{macManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="66976-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="66976-135">Response</span></span>
<span data-ttu-id="66976-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66976-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 137

{
  "value": {
    "@odata.type": "#microsoft.graph.macManagedAppProtection",
    "id": "bb139531-9531-bb13-3195-13bb319513bb"
  }
}
```




