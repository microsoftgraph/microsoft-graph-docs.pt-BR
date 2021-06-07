---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ae034d3dc0ea92e95d61d52fecda09c9627136e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732305"
---
# <a name="update-user"></a><span data-ttu-id="930aa-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="930aa-103">Update user</span></span>

<span data-ttu-id="930aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="930aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="930aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="930aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="930aa-106">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="930aa-106">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="930aa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="930aa-107">Prerequisites</span></span>
<span data-ttu-id="930aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="930aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="930aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="930aa-110">Permission type</span></span>|<span data-ttu-id="930aa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="930aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="930aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="930aa-112">Delegated (work or school account)</span></span>| <span data-ttu-id="930aa-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="930aa-113">_varies by context_</span></span>|
| <span data-ttu-id="930aa-114">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="930aa-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="930aa-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="930aa-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="930aa-116">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="930aa-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="930aa-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="930aa-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="930aa-118">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="930aa-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="930aa-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="930aa-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="930aa-120">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="930aa-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="930aa-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="930aa-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="930aa-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="930aa-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="930aa-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="930aa-123">Not supported.</span></span>|
|<span data-ttu-id="930aa-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="930aa-124">Application</span></span>|<span data-ttu-id="930aa-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="930aa-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="930aa-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="930aa-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="930aa-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="930aa-127">Request headers</span></span>
|<span data-ttu-id="930aa-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="930aa-128">Header</span></span>|<span data-ttu-id="930aa-129">Valor</span><span class="sxs-lookup"><span data-stu-id="930aa-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="930aa-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="930aa-130">Authorization</span></span>|<span data-ttu-id="930aa-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="930aa-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="930aa-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="930aa-132">Accept</span></span>|<span data-ttu-id="930aa-133">application/json</span><span class="sxs-lookup"><span data-stu-id="930aa-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="930aa-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="930aa-134">Request body</span></span>
<span data-ttu-id="930aa-135">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="930aa-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="930aa-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="930aa-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="930aa-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="930aa-137">Property</span></span>|<span data-ttu-id="930aa-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="930aa-138">Type</span></span>|<span data-ttu-id="930aa-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="930aa-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="930aa-140">id</span><span class="sxs-lookup"><span data-stu-id="930aa-140">id</span></span>|<span data-ttu-id="930aa-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="930aa-141">String</span></span>|<span data-ttu-id="930aa-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="930aa-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="930aa-143">**Integração**</span><span class="sxs-lookup"><span data-stu-id="930aa-143">**Onboarding**</span></span>|
|<span data-ttu-id="930aa-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="930aa-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="930aa-145">Int32</span><span class="sxs-lookup"><span data-stu-id="930aa-145">Int32</span></span>|<span data-ttu-id="930aa-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="930aa-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="930aa-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="930aa-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="930aa-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="930aa-148">Response</span></span>
<span data-ttu-id="930aa-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="930aa-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="930aa-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="930aa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="930aa-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="930aa-151">Request</span></span>
<span data-ttu-id="930aa-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="930aa-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="930aa-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="930aa-153">Response</span></span>
<span data-ttu-id="930aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="930aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









