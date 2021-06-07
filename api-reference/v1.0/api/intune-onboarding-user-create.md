---
title: Criar usuário
description: Criar um novo objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdae74bf82fd7d4aeac41b54f0cc87e1b296b0ef
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752844"
---
# <a name="create-user"></a><span data-ttu-id="411a0-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="411a0-103">Create user</span></span>

<span data-ttu-id="411a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="411a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="411a0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="411a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="411a0-106">Criar um novo objeto [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="411a0-106">Create a new [user](../resources/intune-onboarding-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="411a0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="411a0-107">Prerequisites</span></span>
<span data-ttu-id="411a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="411a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="411a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="411a0-110">Permission type</span></span>|<span data-ttu-id="411a0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="411a0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="411a0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="411a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="411a0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="411a0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="411a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="411a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="411a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="411a0-115">Not supported.</span></span>|
|<span data-ttu-id="411a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="411a0-116">Application</span></span>|<span data-ttu-id="411a0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="411a0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="411a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="411a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="411a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="411a0-119">Request headers</span></span>
|<span data-ttu-id="411a0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="411a0-120">Header</span></span>|<span data-ttu-id="411a0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="411a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="411a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="411a0-122">Authorization</span></span>|<span data-ttu-id="411a0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="411a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="411a0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="411a0-124">Accept</span></span>|<span data-ttu-id="411a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="411a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="411a0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="411a0-126">Request body</span></span>
<span data-ttu-id="411a0-127">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="411a0-127">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="411a0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="411a0-128">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="411a0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="411a0-129">Property</span></span>|<span data-ttu-id="411a0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="411a0-130">Type</span></span>|<span data-ttu-id="411a0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="411a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="411a0-132">id</span><span class="sxs-lookup"><span data-stu-id="411a0-132">id</span></span>|<span data-ttu-id="411a0-133">String</span><span class="sxs-lookup"><span data-stu-id="411a0-133">String</span></span>|<span data-ttu-id="411a0-134">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="411a0-134">Unique identifier of the user.</span></span>|
|<span data-ttu-id="411a0-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="411a0-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="411a0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="411a0-136">Int32</span></span>|<span data-ttu-id="411a0-137">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="411a0-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="411a0-138">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="411a0-138">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="411a0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="411a0-139">Response</span></span>
<span data-ttu-id="411a0-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-onboarding-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="411a0-140">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-onboarding-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="411a0-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="411a0-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="411a0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="411a0-142">Request</span></span>
<span data-ttu-id="411a0-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="411a0-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="411a0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="411a0-144">Response</span></span>
<span data-ttu-id="411a0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="411a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```




