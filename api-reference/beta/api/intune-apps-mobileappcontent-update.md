---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d793c25763de7a33cbb18bebc8888d0c5cfd512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838357"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="3a9ce-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3a9ce-103">Update mobileAppContent</span></span>

> <span data-ttu-id="3a9ce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a9ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a9ce-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a9ce-107">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ce-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a9ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a9ce-108">Prerequisites</span></span>
<span data-ttu-id="3a9ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a9ce-111">Permission type</span></span>|<span data-ttu-id="3a9ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a9ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a9ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9ce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9ce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a9ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a9ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-116">Not supported.</span></span>|
|<span data-ttu-id="3a9ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a9ce-117">Application</span></span>|<span data-ttu-id="3a9ce-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a9ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="3a9ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ce-120">Request headers</span></span>
|<span data-ttu-id="3a9ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a9ce-121">Header</span></span>|<span data-ttu-id="3a9ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a9ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a9ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a9ce-123">Authorization</span></span>|<span data-ttu-id="3a9ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a9ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a9ce-125">Accept</span></span>|<span data-ttu-id="3a9ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ce-127">Request body</span></span>
<span data-ttu-id="3a9ce-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ce-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="3a9ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ce-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="3a9ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a9ce-130">Property</span></span>|<span data-ttu-id="3a9ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a9ce-131">Type</span></span>|<span data-ttu-id="3a9ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a9ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a9ce-133">id</span><span class="sxs-lookup"><span data-stu-id="3a9ce-133">id</span></span>|<span data-ttu-id="3a9ce-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a9ce-134">String</span></span>|<span data-ttu-id="3a9ce-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="3a9ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9ce-136">Response</span></span>
<span data-ttu-id="3a9ce-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9ce-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a9ce-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a9ce-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ce-139">Request</span></span>
<span data-ttu-id="3a9ce-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3a9ce-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9ce-141">Response</span></span>
<span data-ttu-id="3a9ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a9ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





