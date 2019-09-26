---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9cbb3874028561cd706ae2f37eb536deb330b81b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193070"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="52331-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="52331-103">Create managedMobileApp</span></span>

> <span data-ttu-id="52331-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52331-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52331-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52331-106">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52331-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52331-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52331-107">Prerequisites</span></span>
<span data-ttu-id="52331-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52331-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52331-110">Permission type</span></span>|<span data-ttu-id="52331-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52331-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52331-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52331-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52331-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52331-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52331-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52331-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52331-115">Not supported.</span></span>|
|<span data-ttu-id="52331-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52331-116">Application</span></span>|<span data-ttu-id="52331-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52331-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52331-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52331-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="52331-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52331-119">Request headers</span></span>
|<span data-ttu-id="52331-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52331-120">Header</span></span>|<span data-ttu-id="52331-121">Valor</span><span class="sxs-lookup"><span data-stu-id="52331-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52331-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="52331-122">Authorization</span></span>|<span data-ttu-id="52331-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52331-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52331-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52331-124">Accept</span></span>|<span data-ttu-id="52331-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52331-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52331-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52331-126">Request body</span></span>
<span data-ttu-id="52331-127">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="52331-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="52331-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="52331-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="52331-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52331-129">Property</span></span>|<span data-ttu-id="52331-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="52331-130">Type</span></span>|<span data-ttu-id="52331-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="52331-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52331-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="52331-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="52331-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="52331-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="52331-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="52331-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="52331-135">id</span><span class="sxs-lookup"><span data-stu-id="52331-135">id</span></span>|<span data-ttu-id="52331-136">String</span><span class="sxs-lookup"><span data-stu-id="52331-136">String</span></span>|<span data-ttu-id="52331-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="52331-137">Key of the entity.</span></span>|
|<span data-ttu-id="52331-138">versão</span><span class="sxs-lookup"><span data-stu-id="52331-138">version</span></span>|<span data-ttu-id="52331-139">String</span><span class="sxs-lookup"><span data-stu-id="52331-139">String</span></span>|<span data-ttu-id="52331-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="52331-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="52331-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="52331-141">Response</span></span>
<span data-ttu-id="52331-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52331-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52331-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52331-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="52331-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52331-144">Request</span></span>
<span data-ttu-id="52331-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52331-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="52331-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="52331-146">Response</span></span>
<span data-ttu-id="52331-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52331-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




