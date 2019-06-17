---
title: Excluir macOsVppApp
description: Exclui macOsVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 723d4118428a2f0ad32a502789cca35abc5be3c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975256"
---
# <a name="delete-macosvppapp"></a><span data-ttu-id="5dccd-103">Excluir macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="5dccd-103">Delete macOsVppApp</span></span>

> <span data-ttu-id="5dccd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dccd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dccd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dccd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dccd-106">Exclui [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dccd-106">Deletes a [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dccd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dccd-107">Prerequisites</span></span>
<span data-ttu-id="5dccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dccd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dccd-110">Permission type</span></span>|<span data-ttu-id="5dccd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dccd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dccd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dccd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5dccd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dccd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5dccd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dccd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dccd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dccd-115">Not supported.</span></span>|
|<span data-ttu-id="5dccd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dccd-116">Application</span></span>|<span data-ttu-id="5dccd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dccd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dccd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dccd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5dccd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dccd-119">Request headers</span></span>
|<span data-ttu-id="5dccd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dccd-120">Header</span></span>|<span data-ttu-id="5dccd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5dccd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dccd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dccd-122">Authorization</span></span>|<span data-ttu-id="5dccd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dccd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dccd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dccd-124">Accept</span></span>|<span data-ttu-id="5dccd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5dccd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dccd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dccd-126">Request body</span></span>
<span data-ttu-id="5dccd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dccd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dccd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dccd-128">Response</span></span>
<span data-ttu-id="5dccd-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5dccd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5dccd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dccd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dccd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dccd-131">Request</span></span>
<span data-ttu-id="5dccd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dccd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="5dccd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dccd-133">Response</span></span>
<span data-ttu-id="5dccd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dccd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





