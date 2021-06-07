---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26d66bc4c9b8c71a0e6fe0146222b55228068fec
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756385"
---
# <a name="update-user"></a><span data-ttu-id="fa462-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="fa462-103">Update user</span></span>

<span data-ttu-id="fa462-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa462-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa462-106">Atualizar as propriedades de um objeto [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="fa462-106">Update the properties of a [user](../resources/intune-mam-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa462-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa462-107">Prerequisites</span></span>
<span data-ttu-id="fa462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa462-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa462-110">Permission type</span></span>|<span data-ttu-id="fa462-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa462-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa462-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa462-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa462-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa462-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa462-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa462-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa462-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa462-115">Not supported.</span></span>|
|<span data-ttu-id="fa462-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa462-116">Application</span></span>|<span data-ttu-id="fa462-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa462-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa462-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa462-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="fa462-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa462-119">Request headers</span></span>
|<span data-ttu-id="fa462-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa462-120">Header</span></span>|<span data-ttu-id="fa462-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa462-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa462-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa462-122">Authorization</span></span>|<span data-ttu-id="fa462-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa462-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa462-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa462-124">Accept</span></span>|<span data-ttu-id="fa462-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa462-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa462-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa462-126">Request body</span></span>
<span data-ttu-id="fa462-127">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="fa462-127">In the request body, supply a JSON representation for the [user](../resources/intune-mam-user.md) object.</span></span>

<span data-ttu-id="fa462-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="fa462-128">The following table shows the properties that are required when you create the [user](../resources/intune-mam-user.md).</span></span>

|<span data-ttu-id="fa462-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa462-129">Property</span></span>|<span data-ttu-id="fa462-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa462-130">Type</span></span>|<span data-ttu-id="fa462-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa462-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa462-132">id</span><span class="sxs-lookup"><span data-stu-id="fa462-132">id</span></span>|<span data-ttu-id="fa462-133">String</span><span class="sxs-lookup"><span data-stu-id="fa462-133">String</span></span>|<span data-ttu-id="fa462-134">O identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa462-134">The user identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="fa462-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa462-135">Response</span></span>
<span data-ttu-id="fa462-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-mam-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa462-136">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-mam-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa462-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa462-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa462-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa462-138">Request</span></span>
<span data-ttu-id="fa462-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa462-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="fa462-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa462-140">Response</span></span>
<span data-ttu-id="fa462-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa462-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




