---
title: Criar userInstallStateSummary
description: Criar um novo objeto userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9493bf685cde5eb142f77f6504317fe05db208ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077797"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="577b1-103">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="577b1-103">Create userInstallStateSummary</span></span>

<span data-ttu-id="577b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="577b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="577b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="577b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="577b1-106">Criar um novo objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="577b1-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="577b1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="577b1-107">Prerequisites</span></span>
<span data-ttu-id="577b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="577b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="577b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="577b1-110">Permission type</span></span>|<span data-ttu-id="577b1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="577b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="577b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="577b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="577b1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="577b1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="577b1-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="577b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="577b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="577b1-115">Not supported.</span></span>|
|<span data-ttu-id="577b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="577b1-116">Application</span></span>|<span data-ttu-id="577b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="577b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="577b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="577b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="577b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="577b1-119">Request headers</span></span>
|<span data-ttu-id="577b1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="577b1-120">Header</span></span>|<span data-ttu-id="577b1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="577b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="577b1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="577b1-122">Authorization</span></span>|<span data-ttu-id="577b1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="577b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="577b1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="577b1-124">Accept</span></span>|<span data-ttu-id="577b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="577b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="577b1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="577b1-126">Request body</span></span>
<span data-ttu-id="577b1-127">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="577b1-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="577b1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="577b1-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="577b1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="577b1-129">Property</span></span>|<span data-ttu-id="577b1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="577b1-130">Type</span></span>|<span data-ttu-id="577b1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="577b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="577b1-132">id</span><span class="sxs-lookup"><span data-stu-id="577b1-132">id</span></span>|<span data-ttu-id="577b1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="577b1-133">String</span></span>|<span data-ttu-id="577b1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="577b1-134">Key of the entity.</span></span>|
|<span data-ttu-id="577b1-135">userName</span><span class="sxs-lookup"><span data-stu-id="577b1-135">userName</span></span>|<span data-ttu-id="577b1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="577b1-136">String</span></span>|<span data-ttu-id="577b1-137">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="577b1-137">User name.</span></span>|
|<span data-ttu-id="577b1-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="577b1-138">installedDeviceCount</span></span>|<span data-ttu-id="577b1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="577b1-139">Int32</span></span>|<span data-ttu-id="577b1-140">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="577b1-140">Installed Device Count.</span></span>|
|<span data-ttu-id="577b1-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="577b1-141">failedDeviceCount</span></span>|<span data-ttu-id="577b1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="577b1-142">Int32</span></span>|<span data-ttu-id="577b1-143">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="577b1-143">Failed Device Count.</span></span>|
|<span data-ttu-id="577b1-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="577b1-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="577b1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="577b1-145">Int32</span></span>|<span data-ttu-id="577b1-146">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="577b1-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="577b1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="577b1-147">Response</span></span>
<span data-ttu-id="577b1-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="577b1-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="577b1-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="577b1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="577b1-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="577b1-150">Request</span></span>
<span data-ttu-id="577b1-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="577b1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="577b1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="577b1-152">Response</span></span>
<span data-ttu-id="577b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="577b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```









