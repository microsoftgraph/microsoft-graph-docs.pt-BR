---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cf1a5d756f46e3986b8131b7726860edb6931ed1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859511"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="25d87-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="25d87-103">Update managedMobileApp</span></span>

> <span data-ttu-id="25d87-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="25d87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25d87-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="25d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25d87-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="25d87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25d87-107">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="25d87-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25d87-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25d87-108">Prerequisites</span></span>
<span data-ttu-id="25d87-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25d87-111">Permission type</span></span>|<span data-ttu-id="25d87-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25d87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d87-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25d87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25d87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25d87-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25d87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25d87-116">Not supported.</span></span>|
|<span data-ttu-id="25d87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25d87-117">Application</span></span>|<span data-ttu-id="25d87-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25d87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25d87-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="25d87-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25d87-120">Request headers</span></span>
|<span data-ttu-id="25d87-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25d87-121">Header</span></span>|<span data-ttu-id="25d87-122">Valor</span><span class="sxs-lookup"><span data-stu-id="25d87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25d87-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="25d87-123">Authorization</span></span>|<span data-ttu-id="25d87-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25d87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25d87-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25d87-125">Accept</span></span>|<span data-ttu-id="25d87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25d87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d87-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25d87-127">Request body</span></span>
<span data-ttu-id="25d87-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="25d87-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="25d87-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="25d87-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="25d87-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25d87-130">Property</span></span>|<span data-ttu-id="25d87-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="25d87-131">Type</span></span>|<span data-ttu-id="25d87-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="25d87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d87-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="25d87-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="25d87-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="25d87-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="25d87-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="25d87-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="25d87-136">id</span><span class="sxs-lookup"><span data-stu-id="25d87-136">id</span></span>|<span data-ttu-id="25d87-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d87-137">String</span></span>|<span data-ttu-id="25d87-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25d87-138">Key of the entity.</span></span>|
|<span data-ttu-id="25d87-139">version</span><span class="sxs-lookup"><span data-stu-id="25d87-139">version</span></span>|<span data-ttu-id="25d87-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d87-140">String</span></span>|<span data-ttu-id="25d87-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="25d87-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="25d87-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="25d87-142">Response</span></span>
<span data-ttu-id="25d87-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25d87-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d87-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25d87-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="25d87-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25d87-145">Request</span></span>
<span data-ttu-id="25d87-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25d87-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 126

{
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="25d87-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="25d87-147">Response</span></span>
<span data-ttu-id="25d87-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25d87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





