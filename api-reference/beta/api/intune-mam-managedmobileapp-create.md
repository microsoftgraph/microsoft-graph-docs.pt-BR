---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18fc30f022feed381257344b4cb9929dca82a319
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141929"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="60543-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="60543-103">Create managedMobileApp</span></span>

<span data-ttu-id="60543-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60543-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60543-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60543-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60543-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60543-107">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="60543-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60543-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60543-108">Prerequisites</span></span>
<span data-ttu-id="60543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60543-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60543-111">Permission type</span></span>|<span data-ttu-id="60543-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60543-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60543-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60543-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60543-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60543-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60543-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60543-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60543-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60543-116">Not supported.</span></span>|
|<span data-ttu-id="60543-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60543-117">Application</span></span>|<span data-ttu-id="60543-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60543-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60543-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60543-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="60543-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60543-120">Request headers</span></span>
|<span data-ttu-id="60543-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60543-121">Header</span></span>|<span data-ttu-id="60543-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60543-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60543-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60543-123">Authorization</span></span>|<span data-ttu-id="60543-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60543-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60543-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60543-125">Accept</span></span>|<span data-ttu-id="60543-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60543-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60543-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60543-127">Request body</span></span>
<span data-ttu-id="60543-128">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="60543-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="60543-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="60543-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="60543-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60543-130">Property</span></span>|<span data-ttu-id="60543-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60543-131">Type</span></span>|<span data-ttu-id="60543-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60543-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60543-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60543-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="60543-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60543-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="60543-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="60543-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="60543-136">id</span><span class="sxs-lookup"><span data-stu-id="60543-136">id</span></span>|<span data-ttu-id="60543-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60543-137">String</span></span>|<span data-ttu-id="60543-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60543-138">Key of the entity.</span></span>|
|<span data-ttu-id="60543-139">versão</span><span class="sxs-lookup"><span data-stu-id="60543-139">version</span></span>|<span data-ttu-id="60543-140">String</span><span class="sxs-lookup"><span data-stu-id="60543-140">String</span></span>|<span data-ttu-id="60543-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="60543-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="60543-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="60543-142">Response</span></span>
<span data-ttu-id="60543-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60543-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60543-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60543-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="60543-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60543-145">Request</span></span>
<span data-ttu-id="60543-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60543-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="60543-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="60543-147">Response</span></span>
<span data-ttu-id="60543-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60543-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 276

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




