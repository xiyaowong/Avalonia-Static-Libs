# Avalonia-Static-Libs

csproj

```xml
<ItemGroup Label="ImportLib">
    <DirectPInvoke Include="libHarfBuzzSharp"/>
    <NativeLibrary Include=".\native\libHarfBuzzSharp.lib" Condition="$(RuntimeIdentifier.StartsWith('win'))"/>
    
    <DirectPInvoke Include="libSkiaSharp"/>
    <NativeLibrary Include=".\native\libSkiaSharp.lib" Condition="$(RuntimeIdentifier.StartsWith('win'))"/>
    
    <DirectPInvoke Include="av_libglesv2"/>
    <NativeLibrary Include=".\native\av_libglesv2.lib" Condition="$(RuntimeIdentifier.StartsWith('win'))"/>
</ItemGroup>
```
