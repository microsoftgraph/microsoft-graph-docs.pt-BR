---
title: Atualizar windowsPhone81AppXBundle
description: Atualize as propriedades de um objeto windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14f221eae60a64629eea3fd5e9a2246a36e76ae3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808593"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="ba4af-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="ba4af-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="ba4af-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ba4af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba4af-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ba4af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba4af-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ba4af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba4af-107">Atualize as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="ba4af-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba4af-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba4af-108">Prerequisites</span></span>
<span data-ttu-id="ba4af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba4af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba4af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba4af-111">Permission type</span></span>|<span data-ttu-id="ba4af-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba4af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba4af-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba4af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba4af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba4af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba4af-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba4af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba4af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba4af-116">Not supported.</span></span>|
|<span data-ttu-id="ba4af-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba4af-117">Application</span></span>|<span data-ttu-id="ba4af-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba4af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba4af-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba4af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ba4af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4af-120">Request headers</span></span>
|<span data-ttu-id="ba4af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba4af-121">Header</span></span>|<span data-ttu-id="ba4af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba4af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba4af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba4af-123">Authorization</span></span>|<span data-ttu-id="ba4af-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba4af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba4af-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba4af-125">Accept</span></span>|<span data-ttu-id="ba4af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba4af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba4af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4af-127">Request body</span></span>
<span data-ttu-id="ba4af-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="ba4af-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="ba4af-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="ba4af-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="ba4af-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba4af-130">Property</span></span>|<span data-ttu-id="ba4af-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba4af-131">Type</span></span>|<span data-ttu-id="ba4af-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba4af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba4af-133">id</span><span class="sxs-lookup"><span data-stu-id="ba4af-133">id</span></span>|<span data-ttu-id="ba4af-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-134">String</span></span>|<span data-ttu-id="ba4af-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-135">Key of the entity.</span></span> <span data-ttu-id="ba4af-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ba4af-137">displayName</span></span>|<span data-ttu-id="ba4af-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-138">String</span></span>|<span data-ttu-id="ba4af-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ba4af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ba4af-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-141">description</span><span class="sxs-lookup"><span data-stu-id="ba4af-141">description</span></span>|<span data-ttu-id="ba4af-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-142">String</span></span>|<span data-ttu-id="ba4af-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-143">The description of the app.</span></span> <span data-ttu-id="ba4af-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ba4af-145">publisher</span></span>|<span data-ttu-id="ba4af-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-146">String</span></span>|<span data-ttu-id="ba4af-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-147">The publisher of the app.</span></span> <span data-ttu-id="ba4af-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ba4af-149">largeIcon</span></span>|[<span data-ttu-id="ba4af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ba4af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ba4af-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ba4af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ba4af-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba4af-153">createdDateTime</span></span>|<span data-ttu-id="ba4af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba4af-154">DateTimeOffset</span></span>|<span data-ttu-id="ba4af-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-155">The date and time the app was created.</span></span> <span data-ttu-id="ba4af-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba4af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ba4af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba4af-158">DateTimeOffset</span></span>|<span data-ttu-id="ba4af-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ba4af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ba4af-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ba4af-161">isFeatured</span></span>|<span data-ttu-id="ba4af-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba4af-162">Boolean</span></span>|<span data-ttu-id="ba4af-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ba4af-164">privacyInformationUrl</span></span>|<span data-ttu-id="ba4af-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-165">String</span></span>|<span data-ttu-id="ba4af-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-166">The privacy statement Url.</span></span> <span data-ttu-id="ba4af-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ba4af-168">informationUrl</span></span>|<span data-ttu-id="ba4af-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-169">String</span></span>|<span data-ttu-id="ba4af-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ba4af-170">The more information Url.</span></span> <span data-ttu-id="ba4af-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-172">owner</span><span class="sxs-lookup"><span data-stu-id="ba4af-172">owner</span></span>|<span data-ttu-id="ba4af-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-173">String</span></span>|<span data-ttu-id="ba4af-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-174">The owner of the app.</span></span> <span data-ttu-id="ba4af-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-176">developer</span><span class="sxs-lookup"><span data-stu-id="ba4af-176">developer</span></span>|<span data-ttu-id="ba4af-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-177">String</span></span>|<span data-ttu-id="ba4af-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-178">The developer of the app.</span></span> <span data-ttu-id="ba4af-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-180">Observações</span><span class="sxs-lookup"><span data-stu-id="ba4af-180">notes</span></span>|<span data-ttu-id="ba4af-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-181">String</span></span>|<span data-ttu-id="ba4af-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-182">Notes for the app.</span></span> <span data-ttu-id="ba4af-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ba4af-184">uploadState</span></span>|<span data-ttu-id="ba4af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ba4af-185">Int32</span></span>|<span data-ttu-id="ba4af-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ba4af-186">The upload state.</span></span> <span data-ttu-id="ba4af-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba4af-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ba4af-188">publishingState</span></span>|[<span data-ttu-id="ba4af-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ba4af-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ba4af-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-190">The publishing state for the app.</span></span> <span data-ttu-id="ba4af-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ba4af-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ba4af-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba4af-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ba4af-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ba4af-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ba4af-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ba4af-194">committedContentVersion</span></span>|<span data-ttu-id="ba4af-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-195">String</span></span>|<span data-ttu-id="ba4af-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ba4af-196">The internal committed content version.</span></span> <span data-ttu-id="ba4af-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba4af-198">fileName</span><span class="sxs-lookup"><span data-stu-id="ba4af-198">fileName</span></span>|<span data-ttu-id="ba4af-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-199">String</span></span>|<span data-ttu-id="ba4af-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ba4af-200">The name of the main Lob application file.</span></span> <span data-ttu-id="ba4af-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba4af-202">size</span><span class="sxs-lookup"><span data-stu-id="ba4af-202">size</span></span>|<span data-ttu-id="ba4af-203">Int64</span><span class="sxs-lookup"><span data-stu-id="ba4af-203">Int64</span></span>|<span data-ttu-id="ba4af-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ba4af-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="ba4af-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba4af-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ba4af-206">applicableArchitectures</span></span>|[<span data-ttu-id="ba4af-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ba4af-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ba4af-208">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ba4af-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ba4af-209">Herdada do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="ba4af-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="ba4af-210">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="ba4af-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ba4af-211">identityName</span><span class="sxs-lookup"><span data-stu-id="ba4af-211">identityName</span></span>|<span data-ttu-id="ba4af-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-212">String</span></span>|<span data-ttu-id="ba4af-213">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-213">The Identity Name.</span></span> <span data-ttu-id="ba4af-214">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ba4af-215">identityPublisherHash</span></span>|<span data-ttu-id="ba4af-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-216">String</span></span>|<span data-ttu-id="ba4af-217">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="ba4af-218">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba4af-219">identityResourceIdentifier</span></span>|<span data-ttu-id="ba4af-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-220">String</span></span>|<span data-ttu-id="ba4af-221">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="ba4af-222">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba4af-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ba4af-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba4af-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ba4af-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ba4af-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="ba4af-226">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba4af-227">phoneProductIdentifier</span></span>|<span data-ttu-id="ba4af-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-228">String</span></span>|<span data-ttu-id="ba4af-229">O identificador de produto do telefone.</span><span class="sxs-lookup"><span data-stu-id="ba4af-229">The Phone Product Identifier.</span></span> <span data-ttu-id="ba4af-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="ba4af-231">phonePublisherId</span></span>|<span data-ttu-id="ba4af-232">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-232">String</span></span>|<span data-ttu-id="ba4af-233">A ID do Publisher. telefone herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ba4af-234">identityVersion</span></span>|<span data-ttu-id="ba4af-235">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-235">String</span></span>|<span data-ttu-id="ba4af-236">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ba4af-236">The identity version.</span></span> <span data-ttu-id="ba4af-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ba4af-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="ba4af-238">appXPackageInformationList</span></span>|<span data-ttu-id="ba4af-239">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="ba4af-240">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="ba4af-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="ba4af-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba4af-241">Response</span></span>
<span data-ttu-id="ba4af-242">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba4af-242">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba4af-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba4af-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba4af-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4af-244">Request</span></span>
<span data-ttu-id="ba4af-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba4af-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2100

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="ba4af-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba4af-246">Response</span></span>
<span data-ttu-id="ba4af-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba4af-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2271

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





