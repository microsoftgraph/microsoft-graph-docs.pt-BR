---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83d4478692c0e4de4205a4b33eb05306bad76563
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751521"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="d7868-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d7868-103">Update managedMobileApp</span></span>

<span data-ttu-id="d7868-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7868-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7868-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7868-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7868-106">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7868-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7868-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7868-107">Prerequisites</span></span>
<span data-ttu-id="d7868-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7868-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7868-110">Permission type</span></span>|<span data-ttu-id="d7868-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7868-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7868-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7868-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7868-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7868-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7868-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7868-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7868-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7868-115">Not supported.</span></span>|
|<span data-ttu-id="d7868-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7868-116">Application</span></span>|<span data-ttu-id="d7868-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7868-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7868-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7868-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d7868-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7868-119">Request headers</span></span>
|<span data-ttu-id="d7868-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7868-120">Header</span></span>|<span data-ttu-id="d7868-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7868-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7868-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7868-122">Authorization</span></span>|<span data-ttu-id="d7868-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7868-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7868-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7868-124">Accept</span></span>|<span data-ttu-id="d7868-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7868-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7868-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7868-126">Request body</span></span>
<span data-ttu-id="d7868-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7868-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="d7868-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7868-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="d7868-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7868-129">Property</span></span>|<span data-ttu-id="d7868-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7868-130">Type</span></span>|<span data-ttu-id="d7868-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7868-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7868-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7868-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="d7868-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7868-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d7868-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="d7868-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d7868-135">id</span><span class="sxs-lookup"><span data-stu-id="d7868-135">id</span></span>|<span data-ttu-id="d7868-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7868-136">String</span></span>|<span data-ttu-id="d7868-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7868-137">Key of the entity.</span></span>|
|<span data-ttu-id="d7868-138">versão</span><span class="sxs-lookup"><span data-stu-id="d7868-138">version</span></span>|<span data-ttu-id="d7868-139">String</span><span class="sxs-lookup"><span data-stu-id="d7868-139">String</span></span>|<span data-ttu-id="d7868-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7868-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d7868-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7868-141">Response</span></span>
<span data-ttu-id="d7868-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7868-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7868-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7868-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7868-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7868-144">Request</span></span>
<span data-ttu-id="d7868-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7868-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="d7868-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7868-146">Response</span></span>
<span data-ttu-id="d7868-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7868-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




