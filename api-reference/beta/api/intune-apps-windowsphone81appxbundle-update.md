---
title: Atualizar windowsPhone81AppXBundle
description: Atualize as propriedades de um objeto windowsPhone81AppXBundle.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bb7f25653f8bf5516b1bdd38eb5b8afaafcefb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393988"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="21723-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="21723-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="21723-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="21723-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21723-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21723-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21723-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="21723-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21723-107">Atualize as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="21723-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21723-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21723-108">Prerequisites</span></span>
<span data-ttu-id="21723-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21723-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21723-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21723-111">Permission type</span></span>|<span data-ttu-id="21723-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21723-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21723-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21723-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21723-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21723-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21723-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21723-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21723-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21723-116">Not supported.</span></span>|
|<span data-ttu-id="21723-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21723-117">Application</span></span>|<span data-ttu-id="21723-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21723-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21723-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21723-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="21723-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21723-120">Request headers</span></span>
|<span data-ttu-id="21723-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21723-121">Header</span></span>|<span data-ttu-id="21723-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21723-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21723-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21723-123">Authorization</span></span>|<span data-ttu-id="21723-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21723-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21723-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21723-125">Accept</span></span>|<span data-ttu-id="21723-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21723-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21723-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21723-127">Request body</span></span>
<span data-ttu-id="21723-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="21723-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="21723-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="21723-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="21723-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21723-130">Property</span></span>|<span data-ttu-id="21723-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21723-131">Type</span></span>|<span data-ttu-id="21723-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21723-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21723-133">id</span><span class="sxs-lookup"><span data-stu-id="21723-133">id</span></span>|<span data-ttu-id="21723-134">String</span><span class="sxs-lookup"><span data-stu-id="21723-134">String</span></span>|<span data-ttu-id="21723-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21723-135">Key of the entity.</span></span> <span data-ttu-id="21723-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-137">displayName</span><span class="sxs-lookup"><span data-stu-id="21723-137">displayName</span></span>|<span data-ttu-id="21723-138">String</span><span class="sxs-lookup"><span data-stu-id="21723-138">String</span></span>|<span data-ttu-id="21723-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="21723-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="21723-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-141">description</span><span class="sxs-lookup"><span data-stu-id="21723-141">description</span></span>|<span data-ttu-id="21723-142">String</span><span class="sxs-lookup"><span data-stu-id="21723-142">String</span></span>|<span data-ttu-id="21723-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-143">The description of the app.</span></span> <span data-ttu-id="21723-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-145">publisher</span><span class="sxs-lookup"><span data-stu-id="21723-145">publisher</span></span>|<span data-ttu-id="21723-146">String</span><span class="sxs-lookup"><span data-stu-id="21723-146">String</span></span>|<span data-ttu-id="21723-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-147">The publisher of the app.</span></span> <span data-ttu-id="21723-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="21723-149">largeIcon</span></span>|[<span data-ttu-id="21723-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21723-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21723-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="21723-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="21723-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21723-153">createdDateTime</span></span>|<span data-ttu-id="21723-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21723-154">DateTimeOffset</span></span>|<span data-ttu-id="21723-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-155">The date and time the app was created.</span></span> <span data-ttu-id="21723-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21723-157">lastModifiedDateTime</span></span>|<span data-ttu-id="21723-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21723-158">DateTimeOffset</span></span>|<span data-ttu-id="21723-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="21723-159">The date and time the app was last modified.</span></span> <span data-ttu-id="21723-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="21723-161">isFeatured</span></span>|<span data-ttu-id="21723-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="21723-162">Boolean</span></span>|<span data-ttu-id="21723-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="21723-164">privacyInformationUrl</span></span>|<span data-ttu-id="21723-165">String</span><span class="sxs-lookup"><span data-stu-id="21723-165">String</span></span>|<span data-ttu-id="21723-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="21723-166">The privacy statement Url.</span></span> <span data-ttu-id="21723-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="21723-168">informationUrl</span></span>|<span data-ttu-id="21723-169">String</span><span class="sxs-lookup"><span data-stu-id="21723-169">String</span></span>|<span data-ttu-id="21723-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="21723-170">The more information Url.</span></span> <span data-ttu-id="21723-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-172">owner</span><span class="sxs-lookup"><span data-stu-id="21723-172">owner</span></span>|<span data-ttu-id="21723-173">String</span><span class="sxs-lookup"><span data-stu-id="21723-173">String</span></span>|<span data-ttu-id="21723-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="21723-174">The owner of the app.</span></span> <span data-ttu-id="21723-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-176">developer</span><span class="sxs-lookup"><span data-stu-id="21723-176">developer</span></span>|<span data-ttu-id="21723-177">String</span><span class="sxs-lookup"><span data-stu-id="21723-177">String</span></span>|<span data-ttu-id="21723-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-178">The developer of the app.</span></span> <span data-ttu-id="21723-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-180">Observações</span><span class="sxs-lookup"><span data-stu-id="21723-180">notes</span></span>|<span data-ttu-id="21723-181">String</span><span class="sxs-lookup"><span data-stu-id="21723-181">String</span></span>|<span data-ttu-id="21723-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-182">Notes for the app.</span></span> <span data-ttu-id="21723-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="21723-184">uploadState</span></span>|<span data-ttu-id="21723-185">Int32</span><span class="sxs-lookup"><span data-stu-id="21723-185">Int32</span></span>|<span data-ttu-id="21723-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="21723-186">The upload state.</span></span> <span data-ttu-id="21723-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="21723-188">publishingState</span></span>|[<span data-ttu-id="21723-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="21723-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="21723-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21723-190">The publishing state for the app.</span></span> <span data-ttu-id="21723-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="21723-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="21723-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21723-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="21723-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="21723-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="21723-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="21723-194">isAssigned</span></span>|<span data-ttu-id="21723-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="21723-195">Boolean</span></span>|<span data-ttu-id="21723-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="21723-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="21723-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21723-198">roleScopeTagIds</span></span>|<span data-ttu-id="21723-199">String collection</span><span class="sxs-lookup"><span data-stu-id="21723-199">String collection</span></span>|<span data-ttu-id="21723-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="21723-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="21723-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21723-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="21723-202">committedContentVersion</span></span>|<span data-ttu-id="21723-203">String</span><span class="sxs-lookup"><span data-stu-id="21723-203">String</span></span>|<span data-ttu-id="21723-204">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="21723-204">The internal committed content version.</span></span> <span data-ttu-id="21723-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="21723-206">fileName</span><span class="sxs-lookup"><span data-stu-id="21723-206">fileName</span></span>|<span data-ttu-id="21723-207">String</span><span class="sxs-lookup"><span data-stu-id="21723-207">String</span></span>|<span data-ttu-id="21723-208">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="21723-208">The name of the main Lob application file.</span></span> <span data-ttu-id="21723-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="21723-210">size</span><span class="sxs-lookup"><span data-stu-id="21723-210">size</span></span>|<span data-ttu-id="21723-211">Int64</span><span class="sxs-lookup"><span data-stu-id="21723-211">Int64</span></span>|<span data-ttu-id="21723-212">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="21723-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="21723-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="21723-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="21723-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="21723-214">applicableArchitectures</span></span>|[<span data-ttu-id="21723-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="21723-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="21723-216">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="21723-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="21723-217">Herdada do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="21723-217">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="21723-218">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="21723-218">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="21723-219">identityName</span><span class="sxs-lookup"><span data-stu-id="21723-219">identityName</span></span>|<span data-ttu-id="21723-220">String</span><span class="sxs-lookup"><span data-stu-id="21723-220">String</span></span>|<span data-ttu-id="21723-221">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="21723-221">The Identity Name.</span></span> <span data-ttu-id="21723-222">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-223">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="21723-223">identityPublisherHash</span></span>|<span data-ttu-id="21723-224">String</span><span class="sxs-lookup"><span data-stu-id="21723-224">String</span></span>|<span data-ttu-id="21723-225">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="21723-225">The Identity Publisher Hash.</span></span> <span data-ttu-id="21723-226">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="21723-227">identityResourceIdentifier</span></span>|<span data-ttu-id="21723-228">String</span><span class="sxs-lookup"><span data-stu-id="21723-228">String</span></span>|<span data-ttu-id="21723-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="21723-229">The Identity Resource Identifier.</span></span> <span data-ttu-id="21723-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="21723-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="21723-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="21723-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="21723-233">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="21723-233">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="21723-234">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-235">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="21723-235">phoneProductIdentifier</span></span>|<span data-ttu-id="21723-236">String</span><span class="sxs-lookup"><span data-stu-id="21723-236">String</span></span>|<span data-ttu-id="21723-237">O identificador de produto do telefone.</span><span class="sxs-lookup"><span data-stu-id="21723-237">The Phone Product Identifier.</span></span> <span data-ttu-id="21723-238">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-239">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="21723-239">phonePublisherId</span></span>|<span data-ttu-id="21723-240">String</span><span class="sxs-lookup"><span data-stu-id="21723-240">String</span></span>|<span data-ttu-id="21723-241">A ID do Publisher. telefone herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-241">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="21723-242">identityVersion</span></span>|<span data-ttu-id="21723-243">String</span><span class="sxs-lookup"><span data-stu-id="21723-243">String</span></span>|<span data-ttu-id="21723-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="21723-244">The identity version.</span></span> <span data-ttu-id="21723-245">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="21723-245">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="21723-246">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="21723-246">appXPackageInformationList</span></span>|<span data-ttu-id="21723-247">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="21723-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="21723-248">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="21723-248">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="21723-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="21723-249">Response</span></span>
<span data-ttu-id="21723-250">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21723-250">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21723-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21723-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="21723-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21723-252">Request</span></span>
<span data-ttu-id="21723-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21723-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2184

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="21723-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="21723-254">Response</span></span>
<span data-ttu-id="21723-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21723-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2356

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```




