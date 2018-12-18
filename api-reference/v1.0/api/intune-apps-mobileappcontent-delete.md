---
title: Excluir mobileAppContent
description: Exclui mobileAppContent.
author: tfitzmac
ms.openlocfilehash: 2675bea2ef0d8e74015267f7b71c0f8f530817fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304680"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="b4d13-103">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4d13-103">Delete mobileAppContent</span></span>

> <span data-ttu-id="b4d13-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4d13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4d13-105">Exclui [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4d13-105">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4d13-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4d13-106">Prerequisites</span></span>
<span data-ttu-id="b4d13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4d13-109">Permission type</span></span>|<span data-ttu-id="b4d13-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4d13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4d13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4d13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4d13-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d13-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4d13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4d13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4d13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4d13-114">Not supported.</span></span>|
|<span data-ttu-id="b4d13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4d13-115">Application</span></span>|<span data-ttu-id="b4d13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4d13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4d13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="b4d13-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d13-118">Request headers</span></span>
|<span data-ttu-id="b4d13-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4d13-119">Header</span></span>|<span data-ttu-id="b4d13-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b4d13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4d13-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4d13-121">Authorization</span></span>|<span data-ttu-id="b4d13-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4d13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4d13-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4d13-123">Accept</span></span>|<span data-ttu-id="b4d13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4d13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d13-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d13-125">Request body</span></span>
<span data-ttu-id="b4d13-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4d13-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d13-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d13-127">Response</span></span>
<span data-ttu-id="b4d13-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4d13-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4d13-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4d13-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4d13-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d13-130">Request</span></span>
<span data-ttu-id="b4d13-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4d13-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="b4d13-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d13-132">Response</span></span>
<span data-ttu-id="b4d13-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4d13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



