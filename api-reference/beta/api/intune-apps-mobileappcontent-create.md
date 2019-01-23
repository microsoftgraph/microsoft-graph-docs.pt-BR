---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82a8e0fdd96235f319685dec5223a358421ea8f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404740"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="dce16-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dce16-103">Create mobileAppContent</span></span>

> <span data-ttu-id="dce16-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dce16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dce16-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dce16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dce16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dce16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce16-107">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="dce16-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dce16-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dce16-108">Prerequisites</span></span>
<span data-ttu-id="dce16-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dce16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dce16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dce16-111">Permission type</span></span>|<span data-ttu-id="dce16-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dce16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dce16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dce16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dce16-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dce16-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dce16-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dce16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dce16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce16-116">Not supported.</span></span>|
|<span data-ttu-id="dce16-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dce16-117">Application</span></span>|<span data-ttu-id="dce16-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dce16-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dce16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="dce16-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dce16-120">Request headers</span></span>
|<span data-ttu-id="dce16-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dce16-121">Header</span></span>|<span data-ttu-id="dce16-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dce16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dce16-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dce16-123">Authorization</span></span>|<span data-ttu-id="dce16-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dce16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dce16-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dce16-125">Accept</span></span>|<span data-ttu-id="dce16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dce16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dce16-127">Request body</span></span>
<span data-ttu-id="dce16-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="dce16-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="dce16-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="dce16-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="dce16-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dce16-130">Property</span></span>|<span data-ttu-id="dce16-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dce16-131">Type</span></span>|<span data-ttu-id="dce16-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dce16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce16-133">id</span><span class="sxs-lookup"><span data-stu-id="dce16-133">id</span></span>|<span data-ttu-id="dce16-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dce16-134">String</span></span>|<span data-ttu-id="dce16-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dce16-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="dce16-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce16-136">Response</span></span>
<span data-ttu-id="dce16-137">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dce16-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce16-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dce16-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dce16-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dce16-139">Request</span></span>
<span data-ttu-id="dce16-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dce16-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="dce16-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce16-141">Response</span></span>
<span data-ttu-id="dce16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dce16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




