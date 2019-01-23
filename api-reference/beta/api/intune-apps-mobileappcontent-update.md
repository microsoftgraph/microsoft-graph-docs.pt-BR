---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 262a7fc48e30e816b07aae963a0951ed4605925d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413371"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="d8357-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d8357-103">Update mobileAppContent</span></span>

> <span data-ttu-id="d8357-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8357-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8357-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8357-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8357-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d8357-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8357-107">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d8357-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8357-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8357-108">Prerequisites</span></span>
<span data-ttu-id="d8357-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8357-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8357-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8357-111">Permission type</span></span>|<span data-ttu-id="d8357-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8357-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8357-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8357-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8357-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8357-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8357-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8357-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8357-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8357-116">Not supported.</span></span>|
|<span data-ttu-id="d8357-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8357-117">Application</span></span>|<span data-ttu-id="d8357-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8357-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8357-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8357-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="d8357-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8357-120">Request headers</span></span>
|<span data-ttu-id="d8357-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8357-121">Header</span></span>|<span data-ttu-id="d8357-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8357-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8357-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8357-123">Authorization</span></span>|<span data-ttu-id="d8357-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8357-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8357-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8357-125">Accept</span></span>|<span data-ttu-id="d8357-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8357-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8357-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8357-127">Request body</span></span>
<span data-ttu-id="d8357-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d8357-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="d8357-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d8357-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="d8357-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8357-130">Property</span></span>|<span data-ttu-id="d8357-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8357-131">Type</span></span>|<span data-ttu-id="d8357-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8357-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8357-133">id</span><span class="sxs-lookup"><span data-stu-id="d8357-133">id</span></span>|<span data-ttu-id="d8357-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8357-134">String</span></span>|<span data-ttu-id="d8357-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8357-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="d8357-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8357-136">Response</span></span>
<span data-ttu-id="d8357-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8357-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8357-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8357-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8357-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8357-139">Request</span></span>
<span data-ttu-id="d8357-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8357-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="d8357-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8357-141">Response</span></span>
<span data-ttu-id="d8357-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8357-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




