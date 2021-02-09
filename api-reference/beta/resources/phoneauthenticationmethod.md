---
title: Tipo de recurso phoneAuthenticationMethod
description: Uma representação de um telefone registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 397d55050cbe0e985075a83527efff45572afe0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156683"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="12065-103">Tipo de recurso phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12065-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="12065-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12065-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12065-105">Uma representação de um telefone registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="12065-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="12065-106">Esse recurso inclui o número de telefone, o tipo de telefone e se o telefone está configurado para o usuário entrar via SMS.</span><span class="sxs-lookup"><span data-stu-id="12065-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="12065-107">Um telefone tem um dos três tipos: celular, celular alternativo ou escritório.</span><span class="sxs-lookup"><span data-stu-id="12065-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="12065-108">Um usuário pode ter um número registrado para cada tipo e deve ter um telefone celular antes de adicionar um celular alternativo.</span><span class="sxs-lookup"><span data-stu-id="12065-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="12065-109">Ao usar um telefone para a autenticação multifatória (MFA) ou para a redefinição de senha de autoatendente (SSPR), o telefone celular é o padrão e o telefone celular alternativo é o backup.</span><span class="sxs-lookup"><span data-stu-id="12065-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="12065-110">Os telefones celulares podem ser usados para sms e chamadas de voz, dependendo das configurações do locatário.</span><span class="sxs-lookup"><span data-stu-id="12065-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="12065-111">Um telefone de escritório só pode receber chamadas de voz, não mensagens SMS.</span><span class="sxs-lookup"><span data-stu-id="12065-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="12065-112">A propriedade de estado de login SMS fornece informações sobre se um número de telefone está pronto ou não para entrar via SMS.</span><span class="sxs-lookup"><span data-stu-id="12065-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="12065-113">A seguir estão os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="12065-113">The following are the possible values.</span></span>

|<span data-ttu-id="12065-114">Valor</span><span class="sxs-lookup"><span data-stu-id="12065-114">Value</span></span>|<span data-ttu-id="12065-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="12065-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="12065-116">Não há suporte para o login principal nesse método de autenticação; por exemplo, a assinatura pode ser habilitada apenas no número de celular principal de um usuário, não no número alternativo.</span><span class="sxs-lookup"><span data-stu-id="12065-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="12065-117">Esse usuário não está habilitado pela política para usar esse método como uma login principal.</span><span class="sxs-lookup"><span data-stu-id="12065-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="12065-118">Esse usuário é habilitado pela política para usar esse método como login principal, mas precisa tomar medidas adicionais para configurá-lo.</span><span class="sxs-lookup"><span data-stu-id="12065-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="12065-119">Este usuário tentou configurar um número de telefone como o número principal de login, mas o número não era exclusivo e não pode ser usado como um nome de login.</span><span class="sxs-lookup"><span data-stu-id="12065-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="12065-120">Esse método de autenticação está pronto para ser usado na login principal.</span><span class="sxs-lookup"><span data-stu-id="12065-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="12065-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="12065-121">Methods</span></span>

| <span data-ttu-id="12065-122">Método</span><span class="sxs-lookup"><span data-stu-id="12065-122">Method</span></span>       | <span data-ttu-id="12065-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12065-123">Return Type</span></span> | <span data-ttu-id="12065-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="12065-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="12065-125">List</span><span class="sxs-lookup"><span data-stu-id="12065-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="12065-126">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12065-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="12065-127">Leia as propriedades e as relações de todos os objetos phoneAuthenticationMethod desse usuário.</span><span class="sxs-lookup"><span data-stu-id="12065-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="12065-128">Get</span><span class="sxs-lookup"><span data-stu-id="12065-128">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="12065-129">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12065-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="12065-130">Leia as propriedades e os relacionamentos do objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="12065-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="12065-131">Update</span><span class="sxs-lookup"><span data-stu-id="12065-131">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="12065-132">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12065-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="12065-133">Atualize o objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="12065-133">Update phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="12065-134">Delete</span><span class="sxs-lookup"><span data-stu-id="12065-134">Delete</span></span>](../api/phoneauthenticationmethod-delete.md) | <span data-ttu-id="12065-135">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="12065-135">None</span></span> | <span data-ttu-id="12065-136">Exclua o objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="12065-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="12065-137">Desabilitar a assinatura de SMS</span><span class="sxs-lookup"><span data-stu-id="12065-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="12065-138">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="12065-138">None</span></span>|<span data-ttu-id="12065-139">Desativar a login por SMS para um usuário.</span><span class="sxs-lookup"><span data-stu-id="12065-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="12065-140">Habilitar a assinatura de SMS</span><span class="sxs-lookup"><span data-stu-id="12065-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="12065-141">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="12065-141">None</span></span>|<span data-ttu-id="12065-142">Ativar a login sms para um usuário.</span><span class="sxs-lookup"><span data-stu-id="12065-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="12065-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12065-143">Properties</span></span>

| <span data-ttu-id="12065-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12065-144">Property</span></span>     | <span data-ttu-id="12065-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="12065-145">Type</span></span>        | <span data-ttu-id="12065-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="12065-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12065-147">id</span><span class="sxs-lookup"><span data-stu-id="12065-147">id</span></span>|<span data-ttu-id="12065-148">String</span><span class="sxs-lookup"><span data-stu-id="12065-148">String</span></span>| <span data-ttu-id="12065-149">O identificador deste telefone registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="12065-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="12065-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12065-150">Read-only.</span></span>|
|<span data-ttu-id="12065-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="12065-151">phoneNumber</span></span>|<span data-ttu-id="12065-152">String</span><span class="sxs-lookup"><span data-stu-id="12065-152">String</span></span>|<span data-ttu-id="12065-153">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="12065-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="12065-154">Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="12065-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="12065-155">Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos.</span><span class="sxs-lookup"><span data-stu-id="12065-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="12065-156">Os números serão rejeitados ao criar/atualizar se não corresponderem ao formato necessário.</span><span class="sxs-lookup"><span data-stu-id="12065-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="12065-157">phoneType</span><span class="sxs-lookup"><span data-stu-id="12065-157">phoneType</span></span>|<span data-ttu-id="12065-158">string</span><span class="sxs-lookup"><span data-stu-id="12065-158">string</span></span>|<span data-ttu-id="12065-159">O tipo deste telefone.</span><span class="sxs-lookup"><span data-stu-id="12065-159">The type of this phone.</span></span> <span data-ttu-id="12065-160">Os valores possíveis `mobile` são: `alternateMobile` , ou `office` .</span><span class="sxs-lookup"><span data-stu-id="12065-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="12065-161">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="12065-161">smsSignInState</span></span>|<span data-ttu-id="12065-162">string</span><span class="sxs-lookup"><span data-stu-id="12065-162">string</span></span>|<span data-ttu-id="12065-163">Se um telefone está pronto para ser usado para entrar por SMS ou não.</span><span class="sxs-lookup"><span data-stu-id="12065-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="12065-164">Os valores possíveis `notSupported` são: `notAllowedByPolicy` , , , ou `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` .</span><span class="sxs-lookup"><span data-stu-id="12065-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12065-165">Relações</span><span class="sxs-lookup"><span data-stu-id="12065-165">Relationships</span></span>

<span data-ttu-id="12065-166">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12065-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12065-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12065-167">JSON representation</span></span>

<span data-ttu-id="12065-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12065-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


