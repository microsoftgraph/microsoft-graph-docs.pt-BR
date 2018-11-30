---
title: Excluir mobileAppContentFile
description: Exclui mobileAppContentFile.
ms.openlocfilehash: db992ee4bbfeeb21f0ccb028659ec5f517fc02ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004668"
---
# <a name="delete-mobileappcontentfile"></a><span data-ttu-id="3534c-103">Excluir mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="3534c-103">Delete mobileAppContentFile</span></span>

> <span data-ttu-id="3534c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3534c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3534c-105">Exclui [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="3534c-105">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3534c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3534c-106">Prerequisites</span></span>
<span data-ttu-id="3534c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3534c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3534c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3534c-109">Permission type</span></span>|<span data-ttu-id="3534c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3534c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3534c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3534c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3534c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3534c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3534c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3534c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3534c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3534c-114">Not supported.</span></span>|
|<span data-ttu-id="3534c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3534c-115">Application</span></span>|<span data-ttu-id="3534c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3534c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3534c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3534c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="3534c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3534c-118">Request headers</span></span>
|<span data-ttu-id="3534c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3534c-119">Header</span></span>|<span data-ttu-id="3534c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3534c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3534c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3534c-121">Authorization</span></span>|<span data-ttu-id="3534c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3534c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3534c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3534c-123">Accept</span></span>|<span data-ttu-id="3534c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3534c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3534c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3534c-125">Request body</span></span>
<span data-ttu-id="3534c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3534c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3534c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3534c-127">Response</span></span>
<span data-ttu-id="3534c-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3534c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3534c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3534c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3534c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3534c-130">Request</span></span>
<span data-ttu-id="3534c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3534c-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="3534c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3534c-132">Response</span></span>
<span data-ttu-id="3534c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3534c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



