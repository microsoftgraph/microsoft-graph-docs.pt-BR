---
title: ação createGooglePlayWebToken
description: Gera um token Web que é usado em um componente incorporável.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95ce74b002f26632945d19ad191edeb76eedd2ae
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762507"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="6f63b-103">ação createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="6f63b-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="6f63b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f63b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f63b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f63b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f63b-106">Gera um token Web que é usado em um componente incorporável.</span><span class="sxs-lookup"><span data-stu-id="6f63b-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f63b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f63b-107">Prerequisites</span></span>
<span data-ttu-id="6f63b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f63b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f63b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f63b-110">Permission type</span></span>|<span data-ttu-id="6f63b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f63b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f63b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f63b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f63b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f63b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f63b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f63b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f63b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f63b-115">Not supported.</span></span>|
|<span data-ttu-id="6f63b-116">Application</span><span class="sxs-lookup"><span data-stu-id="6f63b-116">Application</span></span>|<span data-ttu-id="6f63b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f63b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f63b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f63b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="6f63b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f63b-119">Request headers</span></span>
|<span data-ttu-id="6f63b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f63b-120">Header</span></span>|<span data-ttu-id="6f63b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6f63b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f63b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f63b-122">Authorization</span></span>|<span data-ttu-id="6f63b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f63b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f63b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f63b-124">Accept</span></span>|<span data-ttu-id="6f63b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f63b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f63b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f63b-126">Request body</span></span>
<span data-ttu-id="6f63b-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6f63b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f63b-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6f63b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f63b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f63b-129">Property</span></span>|<span data-ttu-id="6f63b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f63b-130">Type</span></span>|<span data-ttu-id="6f63b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f63b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f63b-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="6f63b-132">parentUri</span></span>|<span data-ttu-id="6f63b-133">String</span><span class="sxs-lookup"><span data-stu-id="6f63b-133">String</span></span>|<span data-ttu-id="6f63b-134">O caminho https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="6f63b-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="6f63b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f63b-135">Response</span></span>
<span data-ttu-id="6f63b-136">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f63b-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f63b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f63b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f63b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f63b-138">Request</span></span>
<span data-ttu-id="6f63b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f63b-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="6f63b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f63b-140">Response</span></span>
<span data-ttu-id="6f63b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f63b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




