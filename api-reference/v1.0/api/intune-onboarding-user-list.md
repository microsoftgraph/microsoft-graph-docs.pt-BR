---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dcb25811cd9ba56959ec8c203f00d95c7a87f15
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751780"
---
# <a name="list-users"></a><span data-ttu-id="fa7c1-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="fa7c1-103">List users</span></span>

<span data-ttu-id="fa7c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa7c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa7c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa7c1-106">Listar propriedades e relações de objetos de [usuário](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-106">List properties and relationships of the [user](../resources/intune-onboarding-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa7c1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa7c1-107">Prerequisites</span></span>
<span data-ttu-id="fa7c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa7c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa7c1-110">Permission type</span></span>|<span data-ttu-id="fa7c1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa7c1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa7c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa7c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa7c1-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa7c1-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa7c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa7c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa7c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-115">Not supported.</span></span>|
|<span data-ttu-id="fa7c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa7c1-116">Application</span></span>|<span data-ttu-id="fa7c1-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa7c1-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa7c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa7c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="fa7c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7c1-119">Request headers</span></span>
|<span data-ttu-id="fa7c1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa7c1-120">Header</span></span>|<span data-ttu-id="fa7c1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa7c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa7c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa7c1-122">Authorization</span></span>|<span data-ttu-id="fa7c1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa7c1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa7c1-124">Accept</span></span>|<span data-ttu-id="fa7c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa7c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa7c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7c1-126">Request body</span></span>
<span data-ttu-id="fa7c1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa7c1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa7c1-128">Response</span></span>
<span data-ttu-id="fa7c1-129">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-onboarding-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-onboarding-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa7c1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa7c1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa7c1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7c1-131">Request</span></span>
<span data-ttu-id="fa7c1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="fa7c1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa7c1-133">Response</span></span>
<span data-ttu-id="fa7c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
      "deviceEnrollmentLimit": 5
    }
  ]
}
```




