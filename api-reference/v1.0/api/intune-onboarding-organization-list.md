---
title: Listar organizations
description: Listar propriedades e relações de objetos de organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 092e8636769b7f1e663ec224609226fc6147de31
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756902"
---
# <a name="list-organizations"></a><span data-ttu-id="efe43-103">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="efe43-103">List organizations</span></span>

<span data-ttu-id="efe43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efe43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efe43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe43-106">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="efe43-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efe43-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efe43-107">Prerequisites</span></span>
<span data-ttu-id="efe43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efe43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efe43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efe43-110">Permission type</span></span>|<span data-ttu-id="efe43-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efe43-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efe43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efe43-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe43-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efe43-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efe43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efe43-115">Not supported.</span></span>|
|<span data-ttu-id="efe43-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efe43-116">Application</span></span>|<span data-ttu-id="efe43-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe43-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe43-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efe43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="efe43-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efe43-119">Request headers</span></span>
|<span data-ttu-id="efe43-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efe43-120">Header</span></span>|<span data-ttu-id="efe43-121">Valor</span><span class="sxs-lookup"><span data-stu-id="efe43-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efe43-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="efe43-122">Authorization</span></span>|<span data-ttu-id="efe43-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efe43-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efe43-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efe43-124">Accept</span></span>|<span data-ttu-id="efe43-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efe43-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe43-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efe43-126">Request body</span></span>
<span data-ttu-id="efe43-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efe43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efe43-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe43-128">Response</span></span>
<span data-ttu-id="efe43-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efe43-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efe43-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efe43-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="efe43-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efe43-131">Request</span></span>
<span data-ttu-id="efe43-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efe43-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="efe43-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe43-133">Response</span></span>
<span data-ttu-id="efe43-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efe43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




