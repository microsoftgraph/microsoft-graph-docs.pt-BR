---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
ms.openlocfilehash: 8aba68926a39a23e8adf0448679cb46ea4b79bb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007097"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="0017e-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="0017e-103">Create mobileAppContent</span></span>

> <span data-ttu-id="0017e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0017e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0017e-105">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="0017e-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0017e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0017e-106">Prerequisites</span></span>
<span data-ttu-id="0017e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0017e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0017e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0017e-109">Permission type</span></span>|<span data-ttu-id="0017e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0017e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0017e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0017e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0017e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0017e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0017e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0017e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0017e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0017e-114">Not supported.</span></span>|
|<span data-ttu-id="0017e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0017e-115">Application</span></span>|<span data-ttu-id="0017e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0017e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0017e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0017e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="0017e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0017e-118">Request headers</span></span>
|<span data-ttu-id="0017e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0017e-119">Header</span></span>|<span data-ttu-id="0017e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0017e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0017e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0017e-121">Authorization</span></span>|<span data-ttu-id="0017e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0017e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0017e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0017e-123">Accept</span></span>|<span data-ttu-id="0017e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0017e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0017e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0017e-125">Request body</span></span>
<span data-ttu-id="0017e-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="0017e-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="0017e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="0017e-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="0017e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0017e-128">Property</span></span>|<span data-ttu-id="0017e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0017e-129">Type</span></span>|<span data-ttu-id="0017e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0017e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0017e-131">id</span><span class="sxs-lookup"><span data-stu-id="0017e-131">id</span></span>|<span data-ttu-id="0017e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0017e-132">String</span></span>|<span data-ttu-id="0017e-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0017e-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="0017e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0017e-134">Response</span></span>
<span data-ttu-id="0017e-135">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0017e-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0017e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0017e-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="0017e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0017e-137">Request</span></span>
<span data-ttu-id="0017e-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0017e-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="0017e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0017e-139">Response</span></span>
<span data-ttu-id="0017e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0017e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



