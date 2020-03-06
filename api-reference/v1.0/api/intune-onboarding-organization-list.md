---
title: Listar organizations
description: Listar propriedades e relações de objetos de organização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 046786b82bc907a99abfb805bc30d5c9b68e0ac4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512416"
---
# <a name="list-organizations"></a><span data-ttu-id="ff28b-103">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="ff28b-103">List organizations</span></span>

<span data-ttu-id="ff28b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff28b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff28b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff28b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff28b-106">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ff28b-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff28b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff28b-107">Prerequisites</span></span>
<span data-ttu-id="ff28b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff28b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff28b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff28b-110">Permission type</span></span>|<span data-ttu-id="ff28b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff28b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff28b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff28b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff28b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff28b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ff28b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff28b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff28b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff28b-115">Not supported.</span></span>|
|<span data-ttu-id="ff28b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff28b-116">Application</span></span>|<span data-ttu-id="ff28b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff28b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff28b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff28b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="ff28b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff28b-119">Request headers</span></span>
|<span data-ttu-id="ff28b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff28b-120">Header</span></span>|<span data-ttu-id="ff28b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff28b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff28b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff28b-122">Authorization</span></span>|<span data-ttu-id="ff28b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff28b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff28b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff28b-124">Accept</span></span>|<span data-ttu-id="ff28b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff28b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff28b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff28b-126">Request body</span></span>
<span data-ttu-id="ff28b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff28b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff28b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff28b-128">Response</span></span>
<span data-ttu-id="ff28b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff28b-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff28b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff28b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff28b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff28b-131">Request</span></span>
<span data-ttu-id="ff28b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff28b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="ff28b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff28b-133">Response</span></span>
<span data-ttu-id="ff28b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff28b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```




