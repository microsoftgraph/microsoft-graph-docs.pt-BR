<span data-ttu-id="2f95f-p105">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="2f95f-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:

| <span data-ttu-id="2f95f-162">Nome</span><span class="sxs-lookup"><span data-stu-id="2f95f-162">Name</span></span>           | <span data-ttu-id="2f95f-163">Resolução</span><span class="sxs-lookup"><span data-stu-id="2f95f-163">Resolution</span></span>  | <span data-ttu-id="2f95f-164">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="2f95f-164">Aspect Ratio</span></span> | <span data-ttu-id="2f95f-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f95f-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="2f95f-166">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="2f95f-166">96 longest</span></span>  | <span data-ttu-id="2f95f-167">Original</span><span class="sxs-lookup"><span data-stu-id="2f95f-167">Original</span></span>     | <span data-ttu-id="2f95f-168">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="2f95f-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="2f95f-169">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="2f95f-169">176 longest</span></span> | <span data-ttu-id="2f95f-170">Original</span><span class="sxs-lookup"><span data-stu-id="2f95f-170">Original</span></span>     | <span data-ttu-id="2f95f-171">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2f95f-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="2f95f-172">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="2f95f-172">800 longest</span></span> | <span data-ttu-id="2f95f-173">Original</span><span class="sxs-lookup"><span data-stu-id="2f95f-173">Original</span></span>     | <span data-ttu-id="2f95f-174">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="2f95f-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <span data-ttu-id="2f95f-175">Comentários</span><span class="sxs-lookup"><span data-stu-id="2f95f-175">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="2f95f-176">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="2f95f-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="2f95f-177">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="2f95f-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
