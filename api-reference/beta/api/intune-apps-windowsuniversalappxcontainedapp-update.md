---
title: Atualizar windowsUniversalAppXContainedApp
description: Atualize as propriedades de um objeto windowsUniversalAppXContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b396d7d1c2995f9e65db63622ad421a481cfe9de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405608"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="05d14-103">Atualizar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="05d14-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="05d14-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="05d14-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05d14-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05d14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05d14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="05d14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05d14-107">Atualize as propriedades de um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="05d14-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05d14-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05d14-108">Prerequisites</span></span>
<span data-ttu-id="05d14-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="05d14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05d14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05d14-111">Permission type</span></span>|<span data-ttu-id="05d14-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05d14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05d14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05d14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05d14-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05d14-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05d14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05d14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05d14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05d14-116">Not supported.</span></span>|
|<span data-ttu-id="05d14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05d14-117">Application</span></span>|<span data-ttu-id="05d14-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05d14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05d14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05d14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="05d14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05d14-120">Request headers</span></span>
|<span data-ttu-id="05d14-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05d14-121">Header</span></span>|<span data-ttu-id="05d14-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05d14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05d14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05d14-123">Authorization</span></span>|<span data-ttu-id="05d14-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05d14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05d14-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05d14-125">Accept</span></span>|<span data-ttu-id="05d14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05d14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05d14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05d14-127">Request body</span></span>
<span data-ttu-id="05d14-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="05d14-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="05d14-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="05d14-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="05d14-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05d14-130">Property</span></span>|<span data-ttu-id="05d14-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05d14-131">Type</span></span>|<span data-ttu-id="05d14-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05d14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05d14-133">id</span><span class="sxs-lookup"><span data-stu-id="05d14-133">id</span></span>|<span data-ttu-id="05d14-134">String</span><span class="sxs-lookup"><span data-stu-id="05d14-134">String</span></span>|<span data-ttu-id="05d14-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05d14-135">Key of the entity.</span></span> <span data-ttu-id="05d14-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="05d14-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="05d14-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="05d14-137">appUserModelId</span></span>|<span data-ttu-id="05d14-138">String</span><span class="sxs-lookup"><span data-stu-id="05d14-138">String</span></span>|<span data-ttu-id="05d14-139">A ID de modelo de usuário do aplicativo do aplicativo de um aplicativo WindowsUniversalAppX contido.</span><span class="sxs-lookup"><span data-stu-id="05d14-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="05d14-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="05d14-140">Response</span></span>
<span data-ttu-id="05d14-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05d14-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05d14-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05d14-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="05d14-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05d14-143">Request</span></span>
<span data-ttu-id="05d14-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05d14-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="05d14-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="05d14-145">Response</span></span>
<span data-ttu-id="05d14-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05d14-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




