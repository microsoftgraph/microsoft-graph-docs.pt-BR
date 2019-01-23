---
title: Excluir microsoftStoreForBusinessApp
description: Exclui microsoftStoreForBusinessApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10143809a63d4749912ce5d0050946f06750ca6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420679"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="dc6bb-103">Excluir microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="dc6bb-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="dc6bb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc6bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc6bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc6bb-107">Exclui [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc6bb-107">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc6bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc6bb-108">Prerequisites</span></span>
<span data-ttu-id="dc6bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc6bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc6bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc6bb-111">Permission type</span></span>|<span data-ttu-id="dc6bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc6bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc6bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc6bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc6bb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc6bb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc6bb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc6bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc6bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-116">Not supported.</span></span>|
|<span data-ttu-id="dc6bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc6bb-117">Application</span></span>|<span data-ttu-id="dc6bb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc6bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc6bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dc6bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6bb-120">Request headers</span></span>
|<span data-ttu-id="dc6bb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc6bb-121">Header</span></span>|<span data-ttu-id="dc6bb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc6bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc6bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc6bb-123">Authorization</span></span>|<span data-ttu-id="dc6bb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc6bb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc6bb-125">Accept</span></span>|<span data-ttu-id="dc6bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc6bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc6bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6bb-127">Request body</span></span>
<span data-ttu-id="dc6bb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc6bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6bb-129">Response</span></span>
<span data-ttu-id="dc6bb-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc6bb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc6bb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc6bb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6bb-132">Request</span></span>
<span data-ttu-id="dc6bb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="dc6bb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6bb-134">Response</span></span>
<span data-ttu-id="dc6bb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc6bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




