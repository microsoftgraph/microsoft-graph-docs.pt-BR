---
title: Listar termsAndConditionsAcceptanceStatuses
description: Listar propriedades e relações dos objetos termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ba97f47e1c9848591de5fdbe6ba2967f319526d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045800"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="0151a-103">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="0151a-103">List termsAndConditionsAcceptanceStatuses</span></span>

<span data-ttu-id="0151a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0151a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0151a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0151a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0151a-106">Listar propriedades e relações dos objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="0151a-106">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0151a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0151a-107">Prerequisites</span></span>
<span data-ttu-id="0151a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0151a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0151a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0151a-110">Permission type</span></span>|<span data-ttu-id="0151a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0151a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0151a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0151a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0151a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0151a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0151a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0151a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0151a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0151a-115">Not supported.</span></span>|
|<span data-ttu-id="0151a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0151a-116">Application</span></span>|<span data-ttu-id="0151a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0151a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0151a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0151a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0151a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-119">Request headers</span></span>
|<span data-ttu-id="0151a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0151a-120">Header</span></span>|<span data-ttu-id="0151a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0151a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0151a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0151a-122">Authorization</span></span>|<span data-ttu-id="0151a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0151a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0151a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0151a-124">Accept</span></span>|<span data-ttu-id="0151a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0151a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0151a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-126">Request body</span></span>
<span data-ttu-id="0151a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0151a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0151a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0151a-128">Response</span></span>
<span data-ttu-id="0151a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0151a-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0151a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0151a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0151a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-131">Request</span></span>
<span data-ttu-id="0151a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0151a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="0151a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0151a-133">Response</span></span>
<span data-ttu-id="0151a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0151a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









