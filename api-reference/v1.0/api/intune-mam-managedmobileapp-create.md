---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d33b518bad8ddec79f08a16aff288b362e6ea7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069747"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="b143f-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b143f-103">Create managedMobileApp</span></span>

<span data-ttu-id="b143f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b143f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b143f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b143f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b143f-106">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b143f-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b143f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b143f-107">Prerequisites</span></span>
<span data-ttu-id="b143f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b143f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b143f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b143f-110">Permission type</span></span>|<span data-ttu-id="b143f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b143f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b143f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b143f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b143f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b143f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b143f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b143f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b143f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b143f-115">Not supported.</span></span>|
|<span data-ttu-id="b143f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b143f-116">Application</span></span>|<span data-ttu-id="b143f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b143f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b143f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b143f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b143f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b143f-119">Request headers</span></span>
|<span data-ttu-id="b143f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b143f-120">Header</span></span>|<span data-ttu-id="b143f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b143f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b143f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b143f-122">Authorization</span></span>|<span data-ttu-id="b143f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b143f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b143f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b143f-124">Accept</span></span>|<span data-ttu-id="b143f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b143f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b143f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b143f-126">Request body</span></span>
<span data-ttu-id="b143f-127">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="b143f-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="b143f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="b143f-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="b143f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b143f-129">Property</span></span>|<span data-ttu-id="b143f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b143f-130">Type</span></span>|<span data-ttu-id="b143f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b143f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b143f-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b143f-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="b143f-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b143f-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b143f-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b143f-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="b143f-135">id</span><span class="sxs-lookup"><span data-stu-id="b143f-135">id</span></span>|<span data-ttu-id="b143f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b143f-136">String</span></span>|<span data-ttu-id="b143f-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b143f-137">Key of the entity.</span></span>|
|<span data-ttu-id="b143f-138">versão</span><span class="sxs-lookup"><span data-stu-id="b143f-138">version</span></span>|<span data-ttu-id="b143f-139">String</span><span class="sxs-lookup"><span data-stu-id="b143f-139">String</span></span>|<span data-ttu-id="b143f-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b143f-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b143f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b143f-141">Response</span></span>
<span data-ttu-id="b143f-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b143f-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b143f-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b143f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b143f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b143f-144">Request</span></span>
<span data-ttu-id="b143f-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b143f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="b143f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b143f-146">Response</span></span>
<span data-ttu-id="b143f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b143f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









