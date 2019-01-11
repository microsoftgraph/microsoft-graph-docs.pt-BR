---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e30d5aee2b5f19275b29f8d1472101c1fa9968ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870398"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="f116e-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f116e-103">Create mobileAppContent</span></span>

> <span data-ttu-id="f116e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f116e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f116e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f116e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f116e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f116e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f116e-107">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="f116e-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f116e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f116e-108">Prerequisites</span></span>
<span data-ttu-id="f116e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f116e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f116e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f116e-111">Permission type</span></span>|<span data-ttu-id="f116e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f116e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f116e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f116e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f116e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f116e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f116e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f116e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f116e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f116e-116">Not supported.</span></span>|
|<span data-ttu-id="f116e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f116e-117">Application</span></span>|<span data-ttu-id="f116e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f116e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f116e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f116e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="f116e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f116e-120">Request headers</span></span>
|<span data-ttu-id="f116e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f116e-121">Header</span></span>|<span data-ttu-id="f116e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f116e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f116e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f116e-123">Authorization</span></span>|<span data-ttu-id="f116e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f116e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f116e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f116e-125">Accept</span></span>|<span data-ttu-id="f116e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f116e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f116e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f116e-127">Request body</span></span>
<span data-ttu-id="f116e-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="f116e-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="f116e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="f116e-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="f116e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f116e-130">Property</span></span>|<span data-ttu-id="f116e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f116e-131">Type</span></span>|<span data-ttu-id="f116e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f116e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f116e-133">id</span><span class="sxs-lookup"><span data-stu-id="f116e-133">id</span></span>|<span data-ttu-id="f116e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f116e-134">String</span></span>|<span data-ttu-id="f116e-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f116e-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="f116e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f116e-136">Response</span></span>
<span data-ttu-id="f116e-137">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f116e-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f116e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f116e-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f116e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f116e-139">Request</span></span>
<span data-ttu-id="f116e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f116e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="f116e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f116e-141">Response</span></span>
<span data-ttu-id="f116e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f116e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





