---
title: Atualizar managedAppOperation
description: Atualizar as propriedades de um objeto managedAppOperation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 376d54159b2b2eba7ca84d29fecf947cc4561bcb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401275"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="17e92-103">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="17e92-103">Update managedAppOperation</span></span>

> <span data-ttu-id="17e92-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="17e92-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17e92-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17e92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17e92-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="17e92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17e92-107">Atualizar as propriedades de um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17e92-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17e92-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17e92-108">Prerequisites</span></span>
<span data-ttu-id="17e92-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17e92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17e92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17e92-111">Permission type</span></span>|<span data-ttu-id="17e92-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17e92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17e92-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17e92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17e92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17e92-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17e92-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17e92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17e92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e92-116">Not supported.</span></span>|
|<span data-ttu-id="17e92-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17e92-117">Application</span></span>|<span data-ttu-id="17e92-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17e92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17e92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="17e92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17e92-120">Request headers</span></span>
|<span data-ttu-id="17e92-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17e92-121">Header</span></span>|<span data-ttu-id="17e92-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17e92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17e92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17e92-123">Authorization</span></span>|<span data-ttu-id="17e92-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17e92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17e92-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17e92-125">Accept</span></span>|<span data-ttu-id="17e92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17e92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17e92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17e92-127">Request body</span></span>
<span data-ttu-id="17e92-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17e92-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="17e92-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17e92-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="17e92-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17e92-130">Property</span></span>|<span data-ttu-id="17e92-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17e92-131">Type</span></span>|<span data-ttu-id="17e92-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17e92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17e92-133">displayName</span><span class="sxs-lookup"><span data-stu-id="17e92-133">displayName</span></span>|<span data-ttu-id="17e92-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17e92-134">String</span></span>|<span data-ttu-id="17e92-135">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="17e92-135">The operation name.</span></span>|
|<span data-ttu-id="17e92-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17e92-136">lastModifiedDateTime</span></span>|<span data-ttu-id="17e92-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17e92-137">DateTimeOffset</span></span>|<span data-ttu-id="17e92-138">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="17e92-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="17e92-139">estado</span><span class="sxs-lookup"><span data-stu-id="17e92-139">state</span></span>|<span data-ttu-id="17e92-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17e92-140">String</span></span>|<span data-ttu-id="17e92-141">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="17e92-141">The current state of the operation</span></span>|
|<span data-ttu-id="17e92-142">id</span><span class="sxs-lookup"><span data-stu-id="17e92-142">id</span></span>|<span data-ttu-id="17e92-143">String</span><span class="sxs-lookup"><span data-stu-id="17e92-143">String</span></span>|<span data-ttu-id="17e92-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17e92-144">Key of the entity.</span></span>|
|<span data-ttu-id="17e92-145">version</span><span class="sxs-lookup"><span data-stu-id="17e92-145">version</span></span>|<span data-ttu-id="17e92-146">String</span><span class="sxs-lookup"><span data-stu-id="17e92-146">String</span></span>|<span data-ttu-id="17e92-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="17e92-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="17e92-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e92-148">Response</span></span>
<span data-ttu-id="17e92-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e92-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17e92-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17e92-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="17e92-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17e92-151">Request</span></span>
<span data-ttu-id="17e92-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17e92-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="17e92-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e92-153">Response</span></span>
<span data-ttu-id="17e92-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17e92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```




