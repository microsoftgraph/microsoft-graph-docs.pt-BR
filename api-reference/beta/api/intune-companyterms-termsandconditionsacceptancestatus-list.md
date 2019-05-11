---
title: Listar termsAndConditionsAcceptanceStatuses
description: Listar propriedades e relações dos objetos termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f6b4318940692a0b1eb5fd04b1f5d094ae83efc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933869"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="e65de-103">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="e65de-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="e65de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e65de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e65de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e65de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e65de-106">Listar propriedades e relações dos objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e65de-106">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e65de-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e65de-107">Prerequisites</span></span>
<span data-ttu-id="e65de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e65de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e65de-110">Permission type</span></span>|<span data-ttu-id="e65de-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e65de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e65de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e65de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e65de-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e65de-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e65de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e65de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e65de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65de-115">Not supported.</span></span>|
|<span data-ttu-id="e65de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e65de-116">Application</span></span>|<span data-ttu-id="e65de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e65de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e65de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e65de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e65de-119">Request headers</span></span>
|<span data-ttu-id="e65de-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e65de-120">Header</span></span>|<span data-ttu-id="e65de-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e65de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e65de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e65de-122">Authorization</span></span>|<span data-ttu-id="e65de-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e65de-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e65de-124">Accept</span></span>|<span data-ttu-id="e65de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e65de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e65de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e65de-126">Request body</span></span>
<span data-ttu-id="e65de-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e65de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e65de-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65de-128">Response</span></span>
<span data-ttu-id="e65de-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e65de-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e65de-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e65de-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e65de-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e65de-131">Request</span></span>
<span data-ttu-id="e65de-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e65de-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="e65de-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65de-133">Response</span></span>
<span data-ttu-id="e65de-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e65de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```




