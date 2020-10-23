---
title: Excluir cartToClassAssociation
description: Exclui cartToClassAssociation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 232e00d2369e31fd5777a2748c451781fdb52b76
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722708"
---
# <a name="delete-carttoclassassociation"></a><span data-ttu-id="78014-103">Excluir cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="78014-103">Delete cartToClassAssociation</span></span>

<span data-ttu-id="78014-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78014-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78014-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78014-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78014-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78014-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78014-107">Exclui [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="78014-107">Deletes a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78014-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78014-108">Prerequisites</span></span>
<span data-ttu-id="78014-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78014-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78014-111">Permission type</span></span>|<span data-ttu-id="78014-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78014-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78014-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78014-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78014-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78014-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78014-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78014-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78014-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78014-116">Not supported.</span></span>|
|<span data-ttu-id="78014-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78014-117">Application</span></span>|<span data-ttu-id="78014-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78014-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78014-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78014-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="78014-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78014-120">Request headers</span></span>
|<span data-ttu-id="78014-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78014-121">Header</span></span>|<span data-ttu-id="78014-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78014-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78014-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78014-123">Authorization</span></span>|<span data-ttu-id="78014-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78014-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78014-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78014-125">Accept</span></span>|<span data-ttu-id="78014-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78014-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78014-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78014-127">Request body</span></span>
<span data-ttu-id="78014-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78014-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="78014-129">Response</span></span>
<span data-ttu-id="78014-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="78014-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78014-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78014-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="78014-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78014-132">Request</span></span>
<span data-ttu-id="78014-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78014-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

### <a name="response"></a><span data-ttu-id="78014-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="78014-134">Response</span></span>
<span data-ttu-id="78014-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78014-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





