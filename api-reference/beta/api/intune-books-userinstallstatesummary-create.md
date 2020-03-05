---
title: Criar userInstallStateSummary
description: Criar um novo objeto userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b07bbf8c6625ed48e89662eba2e253870f60a90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444501"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="2b0d5-103">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="2b0d5-103">Create userInstallStateSummary</span></span>

<span data-ttu-id="2b0d5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b0d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b0d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b0d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b0d5-107">Criar um novo objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2b0d5-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b0d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b0d5-108">Prerequisites</span></span>
<span data-ttu-id="2b0d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b0d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b0d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b0d5-111">Permission type</span></span>|<span data-ttu-id="2b0d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b0d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b0d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b0d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b0d5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b0d5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b0d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b0d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b0d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-116">Not supported.</span></span>|
|<span data-ttu-id="2b0d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b0d5-117">Application</span></span>|<span data-ttu-id="2b0d5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b0d5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b0d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b0d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2b0d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b0d5-120">Request headers</span></span>
|<span data-ttu-id="2b0d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b0d5-121">Header</span></span>|<span data-ttu-id="2b0d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b0d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b0d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b0d5-123">Authorization</span></span>|<span data-ttu-id="2b0d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b0d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b0d5-125">Accept</span></span>|<span data-ttu-id="2b0d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b0d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b0d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b0d5-127">Request body</span></span>
<span data-ttu-id="2b0d5-128">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="2b0d5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="2b0d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b0d5-130">Property</span></span>|<span data-ttu-id="2b0d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b0d5-131">Type</span></span>|<span data-ttu-id="2b0d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b0d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b0d5-133">id</span><span class="sxs-lookup"><span data-stu-id="2b0d5-133">id</span></span>|<span data-ttu-id="2b0d5-134">String</span><span class="sxs-lookup"><span data-stu-id="2b0d5-134">String</span></span>|<span data-ttu-id="2b0d5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-135">Key of the entity.</span></span>|
|<span data-ttu-id="2b0d5-136">userName</span><span class="sxs-lookup"><span data-stu-id="2b0d5-136">userName</span></span>|<span data-ttu-id="2b0d5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b0d5-137">String</span></span>|<span data-ttu-id="2b0d5-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-138">User name.</span></span>|
|<span data-ttu-id="2b0d5-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2b0d5-139">installedDeviceCount</span></span>|<span data-ttu-id="2b0d5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2b0d5-140">Int32</span></span>|<span data-ttu-id="2b0d5-141">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-141">Installed Device Count.</span></span>|
|<span data-ttu-id="2b0d5-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2b0d5-142">failedDeviceCount</span></span>|<span data-ttu-id="2b0d5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2b0d5-143">Int32</span></span>|<span data-ttu-id="2b0d5-144">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-144">Failed Device Count.</span></span>|
|<span data-ttu-id="2b0d5-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2b0d5-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="2b0d5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2b0d5-146">Int32</span></span>|<span data-ttu-id="2b0d5-147">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="2b0d5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b0d5-148">Response</span></span>
<span data-ttu-id="2b0d5-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b0d5-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b0d5-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b0d5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b0d5-151">Request</span></span>
<span data-ttu-id="2b0d5-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="2b0d5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b0d5-153">Response</span></span>
<span data-ttu-id="2b0d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b0d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





