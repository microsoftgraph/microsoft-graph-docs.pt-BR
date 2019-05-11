---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f865b4921157e4591d216e6f55585688939fb61b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903382"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="47623-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="47623-103">Create managedMobileApp</span></span>

> <span data-ttu-id="47623-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47623-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47623-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47623-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47623-106">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47623-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47623-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47623-107">Prerequisites</span></span>
<span data-ttu-id="47623-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47623-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47623-110">Permission type</span></span>|<span data-ttu-id="47623-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47623-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47623-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47623-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47623-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47623-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47623-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47623-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47623-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47623-115">Not supported.</span></span>|
|<span data-ttu-id="47623-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47623-116">Application</span></span>|<span data-ttu-id="47623-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47623-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47623-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47623-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="47623-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47623-119">Request headers</span></span>
|<span data-ttu-id="47623-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47623-120">Header</span></span>|<span data-ttu-id="47623-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47623-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47623-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47623-122">Authorization</span></span>|<span data-ttu-id="47623-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47623-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47623-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47623-124">Accept</span></span>|<span data-ttu-id="47623-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47623-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47623-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47623-126">Request body</span></span>
<span data-ttu-id="47623-127">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="47623-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="47623-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="47623-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="47623-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47623-129">Property</span></span>|<span data-ttu-id="47623-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="47623-130">Type</span></span>|<span data-ttu-id="47623-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="47623-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47623-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="47623-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="47623-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="47623-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="47623-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="47623-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="47623-135">id</span><span class="sxs-lookup"><span data-stu-id="47623-135">id</span></span>|<span data-ttu-id="47623-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47623-136">String</span></span>|<span data-ttu-id="47623-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47623-137">Key of the entity.</span></span>|
|<span data-ttu-id="47623-138">versão</span><span class="sxs-lookup"><span data-stu-id="47623-138">version</span></span>|<span data-ttu-id="47623-139">String</span><span class="sxs-lookup"><span data-stu-id="47623-139">String</span></span>|<span data-ttu-id="47623-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="47623-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="47623-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="47623-141">Response</span></span>
<span data-ttu-id="47623-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47623-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47623-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47623-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="47623-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47623-144">Request</span></span>
<span data-ttu-id="47623-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47623-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47623-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="47623-146">Response</span></span>
<span data-ttu-id="47623-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47623-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




