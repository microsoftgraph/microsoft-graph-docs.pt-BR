---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 25a770b44be68460196113b5f2396cd34f0de6f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980573"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="60a41-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="60a41-103">Update managedMobileApp</span></span>

> <span data-ttu-id="60a41-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60a41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60a41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60a41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60a41-106">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="60a41-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60a41-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60a41-107">Prerequisites</span></span>
<span data-ttu-id="60a41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60a41-110">Permission type</span></span>|<span data-ttu-id="60a41-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60a41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60a41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60a41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60a41-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a41-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60a41-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60a41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60a41-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a41-115">Not supported.</span></span>|
|<span data-ttu-id="60a41-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60a41-116">Application</span></span>|<span data-ttu-id="60a41-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a41-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60a41-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60a41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="60a41-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60a41-119">Request headers</span></span>
|<span data-ttu-id="60a41-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60a41-120">Header</span></span>|<span data-ttu-id="60a41-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60a41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60a41-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60a41-122">Authorization</span></span>|<span data-ttu-id="60a41-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60a41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60a41-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60a41-124">Accept</span></span>|<span data-ttu-id="60a41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60a41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a41-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60a41-126">Request body</span></span>
<span data-ttu-id="60a41-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="60a41-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="60a41-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="60a41-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="60a41-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60a41-129">Property</span></span>|<span data-ttu-id="60a41-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="60a41-130">Type</span></span>|<span data-ttu-id="60a41-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60a41-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60a41-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="60a41-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60a41-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="60a41-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="60a41-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="60a41-135">id</span><span class="sxs-lookup"><span data-stu-id="60a41-135">id</span></span>|<span data-ttu-id="60a41-136">String</span><span class="sxs-lookup"><span data-stu-id="60a41-136">String</span></span>|<span data-ttu-id="60a41-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60a41-137">Key of the entity.</span></span>|
|<span data-ttu-id="60a41-138">versão</span><span class="sxs-lookup"><span data-stu-id="60a41-138">version</span></span>|<span data-ttu-id="60a41-139">String</span><span class="sxs-lookup"><span data-stu-id="60a41-139">String</span></span>|<span data-ttu-id="60a41-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="60a41-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="60a41-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a41-141">Response</span></span>
<span data-ttu-id="60a41-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60a41-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a41-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60a41-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="60a41-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a41-144">Request</span></span>
<span data-ttu-id="60a41-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a41-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="60a41-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a41-146">Response</span></span>
<span data-ttu-id="60a41-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





