---
title: ação createGooglePlayWebToken
description: Gera um token Web que é usado em um componente incorporável.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5dd7881c4c866d0bce10361f28ad4b6f7043b1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012611"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="a8845-103">ação createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="a8845-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="a8845-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8845-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8845-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8845-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8845-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8845-107">Gera um token Web que é usado em um componente incorporável.</span><span class="sxs-lookup"><span data-stu-id="a8845-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8845-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8845-108">Prerequisites</span></span>
<span data-ttu-id="a8845-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8845-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8845-111">Permission type</span></span>|<span data-ttu-id="a8845-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8845-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8845-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8845-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8845-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8845-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8845-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8845-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8845-116">Not supported.</span></span>|
|<span data-ttu-id="a8845-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8845-117">Application</span></span>|<span data-ttu-id="a8845-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8845-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8845-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8845-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="a8845-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8845-120">Request headers</span></span>
|<span data-ttu-id="a8845-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8845-121">Header</span></span>|<span data-ttu-id="a8845-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8845-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8845-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8845-123">Authorization</span></span>|<span data-ttu-id="a8845-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8845-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8845-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8845-125">Accept</span></span>|<span data-ttu-id="a8845-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8845-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8845-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8845-127">Request body</span></span>
<span data-ttu-id="a8845-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a8845-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8845-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a8845-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8845-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8845-130">Property</span></span>|<span data-ttu-id="a8845-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8845-131">Type</span></span>|<span data-ttu-id="a8845-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8845-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8845-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="a8845-133">parentUri</span></span>|<span data-ttu-id="a8845-134">String</span><span class="sxs-lookup"><span data-stu-id="a8845-134">String</span></span>|<span data-ttu-id="a8845-135">O caminho https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="a8845-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="a8845-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8845-136">Response</span></span>
<span data-ttu-id="a8845-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8845-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8845-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8845-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8845-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8845-139">Request</span></span>
<span data-ttu-id="a8845-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8845-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="a8845-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8845-141">Response</span></span>
<span data-ttu-id="a8845-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8845-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```






