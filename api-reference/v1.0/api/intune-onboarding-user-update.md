---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c807a52cf27c53813f82b70c908575b06f94e4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752842"
---
# <a name="update-user"></a><span data-ttu-id="eed3b-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="eed3b-103">Update user</span></span>

<span data-ttu-id="eed3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eed3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eed3b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eed3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed3b-106">Atualizar as propriedades de um objeto [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="eed3b-106">Update the properties of a [user](../resources/intune-onboarding-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eed3b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eed3b-107">Prerequisites</span></span>
<span data-ttu-id="eed3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed3b-110">Permission type</span></span>|<span data-ttu-id="eed3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eed3b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eed3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eed3b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed3b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eed3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eed3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed3b-115">Not supported.</span></span>|
|<span data-ttu-id="eed3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eed3b-116">Application</span></span>|<span data-ttu-id="eed3b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed3b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eed3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eed3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="eed3b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3b-119">Request headers</span></span>
|<span data-ttu-id="eed3b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eed3b-120">Header</span></span>|<span data-ttu-id="eed3b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eed3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eed3b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eed3b-122">Authorization</span></span>|<span data-ttu-id="eed3b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eed3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eed3b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eed3b-124">Accept</span></span>|<span data-ttu-id="eed3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eed3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed3b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3b-126">Request body</span></span>
<span data-ttu-id="eed3b-127">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="eed3b-127">In the request body, supply a JSON representation for the [user](../resources/intune-onboarding-user.md) object.</span></span>

<span data-ttu-id="eed3b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="eed3b-128">The following table shows the properties that are required when you create the [user](../resources/intune-onboarding-user.md).</span></span>

|<span data-ttu-id="eed3b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eed3b-129">Property</span></span>|<span data-ttu-id="eed3b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eed3b-130">Type</span></span>|<span data-ttu-id="eed3b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eed3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed3b-132">id</span><span class="sxs-lookup"><span data-stu-id="eed3b-132">id</span></span>|<span data-ttu-id="eed3b-133">String</span><span class="sxs-lookup"><span data-stu-id="eed3b-133">String</span></span>|<span data-ttu-id="eed3b-134">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="eed3b-134">Unique identifier of the user.</span></span>|
|<span data-ttu-id="eed3b-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="eed3b-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="eed3b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="eed3b-136">Int32</span></span>|<span data-ttu-id="eed3b-137">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="eed3b-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="eed3b-138">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="eed3b-138">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="eed3b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed3b-139">Response</span></span>
<span data-ttu-id="eed3b-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-onboarding-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eed3b-140">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-onboarding-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed3b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed3b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="eed3b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3b-142">Request</span></span>
<span data-ttu-id="eed3b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eed3b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="eed3b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed3b-144">Response</span></span>
<span data-ttu-id="eed3b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eed3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```




