---
title: Atualizar managedEBookCategory
description: Atualize as propriedades de um objeto managedEBookCategory.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 832fb3f2ddc180a88a21d9484057332800e062a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398328"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="c2fe3-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="c2fe3-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="c2fe3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2fe3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2fe3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2fe3-107">Atualize as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c2fe3-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2fe3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2fe3-108">Prerequisites</span></span>
<span data-ttu-id="c2fe3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2fe3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2fe3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2fe3-111">Permission type</span></span>|<span data-ttu-id="c2fe3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2fe3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2fe3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2fe3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2fe3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2fe3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2fe3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2fe3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2fe3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-116">Not supported.</span></span>|
|<span data-ttu-id="c2fe3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fe3-117">Application</span></span>|<span data-ttu-id="c2fe3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2fe3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2fe3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c2fe3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fe3-120">Request headers</span></span>
|<span data-ttu-id="c2fe3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2fe3-121">Header</span></span>|<span data-ttu-id="c2fe3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c2fe3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2fe3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2fe3-123">Authorization</span></span>|<span data-ttu-id="c2fe3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2fe3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2fe3-125">Accept</span></span>|<span data-ttu-id="c2fe3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2fe3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2fe3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fe3-127">Request body</span></span>
<span data-ttu-id="c2fe3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c2fe3-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="c2fe3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c2fe3-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="c2fe3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2fe3-130">Property</span></span>|<span data-ttu-id="c2fe3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2fe3-131">Type</span></span>|<span data-ttu-id="c2fe3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2fe3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2fe3-133">id</span><span class="sxs-lookup"><span data-stu-id="c2fe3-133">id</span></span>|<span data-ttu-id="c2fe3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2fe3-134">String</span></span>|<span data-ttu-id="c2fe3-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-135">The key of the entity.</span></span>|
|<span data-ttu-id="c2fe3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c2fe3-136">displayName</span></span>|<span data-ttu-id="c2fe3-137">String</span><span class="sxs-lookup"><span data-stu-id="c2fe3-137">String</span></span>|<span data-ttu-id="c2fe3-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="c2fe3-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2fe3-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c2fe3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2fe3-140">DateTimeOffset</span></span>|<span data-ttu-id="c2fe3-141">A data e a hora que da última modificação do ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c2fe3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2fe3-142">Response</span></span>
<span data-ttu-id="c2fe3-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2fe3-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2fe3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2fe3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fe3-145">Request</span></span>
<span data-ttu-id="c2fe3-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c2fe3-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2fe3-147">Response</span></span>
<span data-ttu-id="c2fe3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2fe3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




