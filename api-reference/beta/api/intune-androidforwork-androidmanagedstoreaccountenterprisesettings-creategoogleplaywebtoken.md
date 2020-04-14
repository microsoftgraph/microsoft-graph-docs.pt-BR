---
title: ação createGooglePlayWebToken
description: Gera um token Web que é usado em um componente incorporável.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75c705344b1e2d281579a0f70c78a025ee430b65
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418038"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="d88ea-103">ação createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="d88ea-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="d88ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d88ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d88ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d88ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d88ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88ea-107">Gera um token Web que é usado em um componente incorporável.</span><span class="sxs-lookup"><span data-stu-id="d88ea-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d88ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d88ea-108">Prerequisites</span></span>
<span data-ttu-id="d88ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d88ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d88ea-111">Permission type</span></span>|<span data-ttu-id="d88ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d88ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d88ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d88ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d88ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d88ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d88ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d88ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d88ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d88ea-116">Not supported.</span></span>|
|<span data-ttu-id="d88ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d88ea-117">Application</span></span>|<span data-ttu-id="d88ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d88ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d88ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d88ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="d88ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d88ea-120">Request headers</span></span>
|<span data-ttu-id="d88ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d88ea-121">Header</span></span>|<span data-ttu-id="d88ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d88ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d88ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d88ea-123">Authorization</span></span>|<span data-ttu-id="d88ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d88ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d88ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d88ea-125">Accept</span></span>|<span data-ttu-id="d88ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d88ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d88ea-127">Request body</span></span>
<span data-ttu-id="d88ea-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d88ea-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d88ea-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d88ea-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d88ea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d88ea-130">Property</span></span>|<span data-ttu-id="d88ea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d88ea-131">Type</span></span>|<span data-ttu-id="d88ea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d88ea-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="d88ea-133">parentUri</span></span>|<span data-ttu-id="d88ea-134">String</span><span class="sxs-lookup"><span data-stu-id="d88ea-134">String</span></span>|<span data-ttu-id="d88ea-135">O caminho https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="d88ea-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="d88ea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d88ea-136">Response</span></span>
<span data-ttu-id="d88ea-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d88ea-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d88ea-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d88ea-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d88ea-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d88ea-139">Request</span></span>
<span data-ttu-id="d88ea-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d88ea-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="d88ea-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d88ea-141">Response</span></span>
<span data-ttu-id="d88ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d88ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```



