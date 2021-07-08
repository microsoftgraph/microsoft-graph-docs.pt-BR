---
title: Componente de lista de arquivos no microsoft Graph Toolkit
description: O componente de lista de arquivos é usado para exibir uma lista de arquivos mostrando seu ícone e nome
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 816ea4b76a08d089e419aad2a126b7b39c2727b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334777"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0ce50-103">Componente de lista de arquivos no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="0ce50-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0ce50-104">O componente Lista [](/graph/api/resources/onedrive) de Arquivos exibe uma lista de várias pastas e arquivos usando o nome do arquivo/pasta, um ícone e outras propriedades que você especificar.</span><span class="sxs-lookup"><span data-stu-id="0ce50-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="0ce50-105">Esse componente usa o [componente mgt-file.](./file.md)</span><span class="sxs-lookup"><span data-stu-id="0ce50-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="0ce50-106">Você pode especificar uma unidade ou site específico, exibir uma lista de arquivos com base no tipo de insight (tendência, usado ou compartilhado) ou fornecer consultas para uma lista personalizada de arquivos.</span><span class="sxs-lookup"><span data-stu-id="0ce50-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="0ce50-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ce50-107">Example</span></span>

<span data-ttu-id="0ce50-108">O exemplo a seguir exibe um arquivo usando o `mgt-file-list` componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="0ce50-109">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="0ce50-110">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="0ce50-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="0ce50-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ce50-111">Properties</span></span>

<span data-ttu-id="0ce50-112">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="0ce50-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="0ce50-113">Attribute</span></span> | <span data-ttu-id="0ce50-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ce50-114">Property</span></span> | <span data-ttu-id="0ce50-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce50-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="0ce50-116">file-list-query</span><span class="sxs-lookup"><span data-stu-id="0ce50-116">file-list-query</span></span> | <span data-ttu-id="0ce50-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="0ce50-117">fileListQuery</span></span> | <span data-ttu-id="0ce50-118">A consulta completa ou o caminho para a unidade ou site que contém a lista de arquivos a ser renderização.</span><span class="sxs-lookup"><span data-stu-id="0ce50-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="0ce50-119">file-queries</span><span class="sxs-lookup"><span data-stu-id="0ce50-119">file-queries</span></span> | <span data-ttu-id="0ce50-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="0ce50-120">fileQueries</span></span> | <span data-ttu-id="0ce50-121">Uma matriz de consultas de arquivo a serem renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="0ce50-122">nenhuma</span><span class="sxs-lookup"><span data-stu-id="0ce50-122">none</span></span> | <span data-ttu-id="0ce50-123">arquivos</span><span class="sxs-lookup"><span data-stu-id="0ce50-123">files</span></span> | <span data-ttu-id="0ce50-124">Uma matriz de arquivos para obter ou definir a lista de arquivos renderizados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="0ce50-125">Use isso para acessar os arquivos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="0ce50-126">De definir esse valor para carregar seus próprios arquivos.</span><span class="sxs-lookup"><span data-stu-id="0ce50-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="0ce50-127">tipo de insight</span><span class="sxs-lookup"><span data-stu-id="0ce50-127">insight-type</span></span> | <span data-ttu-id="0ce50-128">insightType</span><span class="sxs-lookup"><span data-stu-id="0ce50-128">insightType</span></span> | <span data-ttu-id="0ce50-129">Definido para mostrar os arquivos de tendência, usados ou compartilhados do usuário.</span><span class="sxs-lookup"><span data-stu-id="0ce50-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="0ce50-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="0ce50-130">drive-id</span></span> | <span data-ttu-id="0ce50-131">driveId</span><span class="sxs-lookup"><span data-stu-id="0ce50-131">driveId</span></span> | <span data-ttu-id="0ce50-132">ID da unidade à que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="0ce50-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="0ce50-133">Também deve fornecer um `item-id` ou `item-path` .</span><span class="sxs-lookup"><span data-stu-id="0ce50-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="0ce50-134">group-id</span><span class="sxs-lookup"><span data-stu-id="0ce50-134">group-id</span></span> | <span data-ttu-id="0ce50-135">groupId</span><span class="sxs-lookup"><span data-stu-id="0ce50-135">groupId</span></span> | <span data-ttu-id="0ce50-136">ID do grupo ao que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="0ce50-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="0ce50-137">Também deve fornecer um `item-id` ou `item-path` .</span><span class="sxs-lookup"><span data-stu-id="0ce50-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="0ce50-138">site-id</span><span class="sxs-lookup"><span data-stu-id="0ce50-138">site-id</span></span> | <span data-ttu-id="0ce50-139">siteId</span><span class="sxs-lookup"><span data-stu-id="0ce50-139">siteId</span></span> | <span data-ttu-id="0ce50-140">ID do site ao que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="0ce50-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="0ce50-141">Também deve fornecer um `{item-id}` ou `{item-path}` .</span><span class="sxs-lookup"><span data-stu-id="0ce50-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="0ce50-142">Forneça `{list-id}` se você estiver fazendo referência a um arquivo de uma lista específica.</span><span class="sxs-lookup"><span data-stu-id="0ce50-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="0ce50-143">item-id</span><span class="sxs-lookup"><span data-stu-id="0ce50-143">item-id</span></span> | <span data-ttu-id="0ce50-144">itemId</span><span class="sxs-lookup"><span data-stu-id="0ce50-144">itemId</span></span> | <span data-ttu-id="0ce50-145">ID da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ce50-145">ID of the folder.</span></span> <span data-ttu-id="0ce50-146">A consulta padrão é `/me/drive/items` .</span><span class="sxs-lookup"><span data-stu-id="0ce50-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="0ce50-147">Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico.</span><span class="sxs-lookup"><span data-stu-id="0ce50-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="0ce50-148">item-path</span><span class="sxs-lookup"><span data-stu-id="0ce50-148">item-path</span></span> | <span data-ttu-id="0ce50-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="0ce50-149">itemPath</span></span> | <span data-ttu-id="0ce50-150">Caminho do item da pasta (em relação à raiz).</span><span class="sxs-lookup"><span data-stu-id="0ce50-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="0ce50-151">A consulta padrão é `/me/drive/root` .</span><span class="sxs-lookup"><span data-stu-id="0ce50-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="0ce50-152">Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico.</span><span class="sxs-lookup"><span data-stu-id="0ce50-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="0ce50-153">tamanho da página</span><span class="sxs-lookup"><span data-stu-id="0ce50-153">page-size</span></span> | <span data-ttu-id="0ce50-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="0ce50-154">pageSize</span></span> | <span data-ttu-id="0ce50-155">Um valor de número para indicar o número máximo de arquivos a renderizar em cada página.</span><span class="sxs-lookup"><span data-stu-id="0ce50-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="0ce50-156">file-extensions</span><span class="sxs-lookup"><span data-stu-id="0ce50-156">file-extensions</span></span> | <span data-ttu-id="0ce50-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="0ce50-157">fileExtensions</span></span> | <span data-ttu-id="0ce50-158">Uma matriz de extensões de arquivo usadas para filtrar arquivos para mostrar.</span><span class="sxs-lookup"><span data-stu-id="0ce50-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="0ce50-159">hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="0ce50-159">hide-more-files-button</span></span> | <span data-ttu-id="0ce50-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="0ce50-160">hideMoreFilesButton</span></span> | <span data-ttu-id="0ce50-161">Um booleano para indicar se é preciso mostrar um botão para renderizar mais arquivos.</span><span class="sxs-lookup"><span data-stu-id="0ce50-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="0ce50-162">O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="0ce50-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="0ce50-163">O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma pasta fornecendo a id da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ce50-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="0ce50-164">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um grupo fornecendo a id do grupo e o caminho da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ce50-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="0ce50-165">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um usuário, fornecendo a ID do usuário e a id da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ce50-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="0ce50-166">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos fornecendo o tipo de insight.</span><span class="sxs-lookup"><span data-stu-id="0ce50-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a><span data-ttu-id="0ce50-167">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ce50-167">Methods</span></span>
| <span data-ttu-id="0ce50-168">Método</span><span class="sxs-lookup"><span data-stu-id="0ce50-168">Method</span></span> | <span data-ttu-id="0ce50-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce50-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="0ce50-170">reload(clearCache = false)</span><span class="sxs-lookup"><span data-stu-id="0ce50-170">reload(clearCache = false)</span></span> | <span data-ttu-id="0ce50-171">Chame o método para recarregar o componente com novos dados potenciais com base em suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0ce50-171">Call the method to reload the component with potential new data based on its properties.</span></span> <span data-ttu-id="0ce50-172">Passe `true` para limpar o cache antes de recarregar.</span><span class="sxs-lookup"><span data-stu-id="0ce50-172">Pass `true` to clear the cache before reloading.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="0ce50-173">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="0ce50-173">CSS custom properties</span></span>

<span data-ttu-id="0ce50-174">O `mgt-file-list` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="0ce50-174">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

<span data-ttu-id="0ce50-175">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="0ce50-175">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="0ce50-176">ApIs Graph Microsoft e permissões</span><span class="sxs-lookup"><span data-stu-id="0ce50-176">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="0ce50-177">Configuração</span><span class="sxs-lookup"><span data-stu-id="0ce50-177">Configuration</span></span> | <span data-ttu-id="0ce50-178">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ce50-178">Permissions</span></span> | <span data-ttu-id="0ce50-179">API</span><span class="sxs-lookup"><span data-stu-id="0ce50-179">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="0ce50-180">Padrão (nenhum identificador ou consulta fornecida)</span><span class="sxs-lookup"><span data-stu-id="0ce50-180">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="0ce50-181">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children` |
| <span data-ttu-id="0ce50-182">Fornecer `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-182">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="0ce50-183">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="0ce50-184">Fornecer `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-184">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="0ce50-185">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="0ce50-186">Fornecer SOMENTE `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-186">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="0ce50-187">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` |
| <span data-ttu-id="0ce50-188">Fornecer `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-188">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="0ce50-189">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="0ce50-190">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-190">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="0ce50-191">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="0ce50-192">Fornecer `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-192">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="0ce50-193">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="0ce50-194">Fornecer `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-194">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="0ce50-195">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="0ce50-196">Fornecer `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-196">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="0ce50-197">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="0ce50-198">Fornecer `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-198">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="0ce50-199">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="0ce50-200">Fornecer somente `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="0ce50-200">Provide only `{item-path}`</span></span> | <span data-ttu-id="0ce50-201">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="0ce50-202">`insight-type` é definido como tendência</span><span class="sxs-lookup"><span data-stu-id="0ce50-202">`insight-type` is set to trending</span></span> | <span data-ttu-id="0ce50-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-203">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="0ce50-204">Fornecer `{user-id or upn}` AND está definido `insight-type` como `trending`</span><span class="sxs-lookup"><span data-stu-id="0ce50-204">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="0ce50-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-205">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` |
| <span data-ttu-id="0ce50-206">`insight-type` está definido como `used`</span><span class="sxs-lookup"><span data-stu-id="0ce50-206">`insight-type` is set to `used`</span></span> | <span data-ttu-id="0ce50-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-207">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="0ce50-208">Fornecer `{user-id or upn}` AND está definido `insight-type` como `used`</span><span class="sxs-lookup"><span data-stu-id="0ce50-208">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="0ce50-209">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-209">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="0ce50-210">`insight-type` é definido como compartilhado</span><span class="sxs-lookup"><span data-stu-id="0ce50-210">`insight-type` is set to shared</span></span> | <span data-ttu-id="0ce50-211">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-211">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="0ce50-212">Fornecer `{user-id or upn}` AND está definido `insight-type` como `shared`</span><span class="sxs-lookup"><span data-stu-id="0ce50-212">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="0ce50-213">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce50-213">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="0ce50-214">Eventos</span><span class="sxs-lookup"><span data-stu-id="0ce50-214">Events</span></span>

<span data-ttu-id="0ce50-215">Evento</span><span class="sxs-lookup"><span data-stu-id="0ce50-215">Event</span></span> | <span data-ttu-id="0ce50-216">Quando é emitido</span><span class="sxs-lookup"><span data-stu-id="0ce50-216">When is it emitted</span></span> | <span data-ttu-id="0ce50-217">Dados personalizados</span><span class="sxs-lookup"><span data-stu-id="0ce50-217">Custom data</span></span> | <span data-ttu-id="0ce50-218">Cancelável</span><span class="sxs-lookup"><span data-stu-id="0ce50-218">Cancelable</span></span> | <span data-ttu-id="0ce50-219">Bolhas</span><span class="sxs-lookup"><span data-stu-id="0ce50-219">Bubbles</span></span> | <span data-ttu-id="0ce50-220">Funciona com modelo personalizado</span><span class="sxs-lookup"><span data-stu-id="0ce50-220">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`itemClick` | <span data-ttu-id="0ce50-221">Disparado quando o usuário clica em um arquivo.</span><span class="sxs-lookup"><span data-stu-id="0ce50-221">Fired when the user clicks a file.</span></span> | <span data-ttu-id="0ce50-222">Arquivo [selecionado](/graph/api/resources/driveItem)</span><span class="sxs-lookup"><span data-stu-id="0ce50-222">Selected [file](/graph/api/resources/driveItem)</span></span> | <span data-ttu-id="0ce50-223">Não</span><span class="sxs-lookup"><span data-stu-id="0ce50-223">No</span></span> | <span data-ttu-id="0ce50-224">Não</span><span class="sxs-lookup"><span data-stu-id="0ce50-224">No</span></span> | <span data-ttu-id="0ce50-225">Sim, com modelo de **arquivo** personalizado</span><span class="sxs-lookup"><span data-stu-id="0ce50-225">Yes, with custom **file** template</span></span>

<span data-ttu-id="0ce50-226">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="0ce50-226">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="0ce50-227">Modelos</span><span class="sxs-lookup"><span data-stu-id="0ce50-227">Templates</span></span>

<span data-ttu-id="0ce50-228">O `mgt-file-list` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="0ce50-228">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="0ce50-229">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos tipos de dados `<template>` `data-type` listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0ce50-229">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="0ce50-230">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="0ce50-230">Data type</span></span> | <span data-ttu-id="0ce50-231">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="0ce50-231">Data context</span></span> | <span data-ttu-id="0ce50-232">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce50-232">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="0ce50-233">Padrão.</span><span class="sxs-lookup"><span data-stu-id="0ce50-233">default</span></span> | <span data-ttu-id="0ce50-234">`files`: lista de objetos de arquivo</span><span class="sxs-lookup"><span data-stu-id="0ce50-234">`files`: list of file objects</span></span> | <span data-ttu-id="0ce50-235">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="0ce50-235">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="0ce50-236">file</span><span class="sxs-lookup"><span data-stu-id="0ce50-236">file</span></span> | <span data-ttu-id="0ce50-237">`file`: objeto file</span><span class="sxs-lookup"><span data-stu-id="0ce50-237">`file`: file object</span></span> | <span data-ttu-id="0ce50-238">O modelo usado para renderizar cada arquivo.</span><span class="sxs-lookup"><span data-stu-id="0ce50-238">The template used to render each file.</span></span> |
| <span data-ttu-id="0ce50-239">no-data</span><span class="sxs-lookup"><span data-stu-id="0ce50-239">no-data</span></span> | <span data-ttu-id="0ce50-240">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="0ce50-240">No data context is passed</span></span> | <span data-ttu-id="0ce50-241">O modelo usado quando nenhum dado está disponível.</span><span class="sxs-lookup"><span data-stu-id="0ce50-241">The template used when no data is available.</span></span> |
| <span data-ttu-id="0ce50-242">loading</span><span class="sxs-lookup"><span data-stu-id="0ce50-242">loading</span></span> | <span data-ttu-id="0ce50-243">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="0ce50-243">No data context is passed</span></span> | <span data-ttu-id="0ce50-244">O modelo usado enquanto o componente carrega o estado.</span><span class="sxs-lookup"><span data-stu-id="0ce50-244">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="0ce50-245">Autenticação</span><span class="sxs-lookup"><span data-stu-id="0ce50-245">Authentication</span></span>

<span data-ttu-id="0ce50-246">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="0ce50-246">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="0ce50-247">Cache</span><span class="sxs-lookup"><span data-stu-id="0ce50-247">Cache</span></span>

|<span data-ttu-id="0ce50-248">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="0ce50-248">Object store</span></span>|<span data-ttu-id="0ce50-249">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="0ce50-249">Cached data</span></span>|<span data-ttu-id="0ce50-250">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ce50-250">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="0ce50-251">Lista de listas de arquivos</span><span class="sxs-lookup"><span data-stu-id="0ce50-251">List of file lists</span></span>|<span data-ttu-id="0ce50-252">Lista de cache padrão para armazenar listas de arquivos.</span><span class="sxs-lookup"><span data-stu-id="0ce50-252">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="0ce50-253">Lista de listas de arquivos de insight</span><span class="sxs-lookup"><span data-stu-id="0ce50-253">List of insight file lists</span></span>|<span data-ttu-id="0ce50-254">Usado quando `insightType` fornecido.</span><span class="sxs-lookup"><span data-stu-id="0ce50-254">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="0ce50-255">O `mgt-file-list` componente também usa o armazenamento de objetos em `fileQueries` `mgt-file` IndexedDB para armazenar arquivos em cache quando `fileQueries` é fornecido.</span><span class="sxs-lookup"><span data-stu-id="0ce50-255">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="0ce50-256">Para obter detalhes sobre como configurar o cache, [consulte Caching](../customize-components/cache.md).</span><span class="sxs-lookup"><span data-stu-id="0ce50-256">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>