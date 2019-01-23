---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 758696dd92361d1d362b520de2963f898405826d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392504"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="fdbf0-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="fdbf0-103">Update managedMobileApp</span></span>

> <span data-ttu-id="fdbf0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fdbf0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdbf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdbf0-107">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fdbf0-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdbf0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdbf0-108">Prerequisites</span></span>
<span data-ttu-id="fdbf0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdbf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fdbf0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdbf0-111">Permission type</span></span>|<span data-ttu-id="fdbf0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdbf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdbf0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdbf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdbf0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdbf0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fdbf0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdbf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdbf0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-116">Not supported.</span></span>|
|<span data-ttu-id="fdbf0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdbf0-117">Application</span></span>|<span data-ttu-id="fdbf0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdbf0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdbf0-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fdbf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdbf0-120">Request headers</span></span>
|<span data-ttu-id="fdbf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdbf0-121">Header</span></span>|<span data-ttu-id="fdbf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdbf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdbf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdbf0-123">Authorization</span></span>|<span data-ttu-id="fdbf0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdbf0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdbf0-125">Accept</span></span>|<span data-ttu-id="fdbf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdbf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdbf0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdbf0-127">Request body</span></span>
<span data-ttu-id="fdbf0-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fdbf0-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="fdbf0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fdbf0-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="fdbf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdbf0-130">Property</span></span>|<span data-ttu-id="fdbf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdbf0-131">Type</span></span>|<span data-ttu-id="fdbf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdbf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdbf0-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fdbf0-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="fdbf0-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fdbf0-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fdbf0-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="fdbf0-136">id</span><span class="sxs-lookup"><span data-stu-id="fdbf0-136">id</span></span>|<span data-ttu-id="fdbf0-137">String</span><span class="sxs-lookup"><span data-stu-id="fdbf0-137">String</span></span>|<span data-ttu-id="fdbf0-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-138">Key of the entity.</span></span>|
|<span data-ttu-id="fdbf0-139">version</span><span class="sxs-lookup"><span data-stu-id="fdbf0-139">version</span></span>|<span data-ttu-id="fdbf0-140">String</span><span class="sxs-lookup"><span data-stu-id="fdbf0-140">String</span></span>|<span data-ttu-id="fdbf0-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fdbf0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdbf0-142">Response</span></span>
<span data-ttu-id="fdbf0-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdbf0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdbf0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdbf0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdbf0-145">Request</span></span>
<span data-ttu-id="fdbf0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdbf0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdbf0-147">Response</span></span>
<span data-ttu-id="fdbf0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdbf0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




