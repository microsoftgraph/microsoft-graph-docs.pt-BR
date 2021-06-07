---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2fba2afd42a4daeeec10a810c4769b0077a6c7ac
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752843"
---
# <a name="get-user"></a><span data-ttu-id="44e0b-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="44e0b-103">Get user</span></span>

<span data-ttu-id="44e0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44e0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44e0b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44e0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44e0b-106">Leia as propriedades e as relações do objeto [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="44e0b-106">Read properties and relationships of the [user](../resources/intune-onboarding-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44e0b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44e0b-107">Prerequisites</span></span>
<span data-ttu-id="44e0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44e0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44e0b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44e0b-110">Permission type</span></span>|<span data-ttu-id="44e0b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44e0b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44e0b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44e0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44e0b-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e0b-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44e0b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44e0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44e0b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44e0b-115">Not supported.</span></span>|
|<span data-ttu-id="44e0b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44e0b-116">Application</span></span>|<span data-ttu-id="44e0b-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e0b-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44e0b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44e0b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44e0b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44e0b-119">Optional query parameters</span></span>
<span data-ttu-id="44e0b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44e0b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44e0b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44e0b-121">Request headers</span></span>
|<span data-ttu-id="44e0b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44e0b-122">Header</span></span>|<span data-ttu-id="44e0b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="44e0b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44e0b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="44e0b-124">Authorization</span></span>|<span data-ttu-id="44e0b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44e0b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44e0b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44e0b-126">Accept</span></span>|<span data-ttu-id="44e0b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="44e0b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44e0b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44e0b-128">Request body</span></span>
<span data-ttu-id="44e0b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44e0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44e0b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="44e0b-130">Response</span></span>
<span data-ttu-id="44e0b-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-onboarding-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44e0b-131">If successful, this method returns a `200 OK` response code and [user](../resources/intune-onboarding-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e0b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44e0b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="44e0b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44e0b-133">Request</span></span>
<span data-ttu-id="44e0b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44e0b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="44e0b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="44e0b-135">Response</span></span>
<span data-ttu-id="44e0b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44e0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
    "deviceEnrollmentLimit": 5
  }
}
```




