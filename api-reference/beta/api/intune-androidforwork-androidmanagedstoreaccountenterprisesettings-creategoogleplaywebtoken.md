---
title: ação createGooglePlayWebToken
description: Gera um token Web que é usado em um componente incorporável.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6452726d6478ee6a7226887156def457d76f3f5f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39927479"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="65efb-103">ação createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="65efb-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="65efb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65efb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65efb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65efb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65efb-106">Gera um token Web que é usado em um componente incorporável.</span><span class="sxs-lookup"><span data-stu-id="65efb-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65efb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65efb-107">Prerequisites</span></span>
<span data-ttu-id="65efb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65efb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65efb-110">Permission type</span></span>|<span data-ttu-id="65efb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65efb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65efb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65efb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65efb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65efb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65efb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65efb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65efb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65efb-115">Not supported.</span></span>|
|<span data-ttu-id="65efb-116">Application</span><span class="sxs-lookup"><span data-stu-id="65efb-116">Application</span></span>|<span data-ttu-id="65efb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65efb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65efb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65efb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="65efb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65efb-119">Request headers</span></span>
|<span data-ttu-id="65efb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65efb-120">Header</span></span>|<span data-ttu-id="65efb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="65efb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65efb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="65efb-122">Authorization</span></span>|<span data-ttu-id="65efb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65efb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65efb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65efb-124">Accept</span></span>|<span data-ttu-id="65efb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65efb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65efb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65efb-126">Request body</span></span>
<span data-ttu-id="65efb-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="65efb-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="65efb-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="65efb-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="65efb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65efb-129">Property</span></span>|<span data-ttu-id="65efb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="65efb-130">Type</span></span>|<span data-ttu-id="65efb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="65efb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65efb-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="65efb-132">parentUri</span></span>|<span data-ttu-id="65efb-133">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="65efb-133">String</span></span>|<span data-ttu-id="65efb-134">O caminho https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="65efb-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="65efb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="65efb-135">Response</span></span>
<span data-ttu-id="65efb-136">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65efb-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65efb-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65efb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="65efb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65efb-138">Request</span></span>
<span data-ttu-id="65efb-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65efb-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="65efb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="65efb-140">Response</span></span>
<span data-ttu-id="65efb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65efb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





